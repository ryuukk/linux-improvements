# Better text rendering

Chromium passes wrong gamma correction values to skia, wich resulsts on poor text rendering on dark themes, specially on small texts when using a non retina screen, eg: 1080p screen 

You can see a test/comparison here: [comparison](chromium-patch-compare/)

Patch chromium with: 

```diff
--- a/skia/BUILD.gn
+++ b/skia/BUILD.gn
@@ -150,12 +150,19 @@
   }
 
   # Settings for text blitting, chosen to approximate the system browser.
-  if (is_linux || is_chromeos) {
+  if (is_chromeos) {
     defines += [
       "SK_GAMMA_EXPONENT=1.2",
       "SK_GAMMA_CONTRAST=0.2",
     ]
-  } else if (is_android) {
+  } else if (is_linux) {
+    defines += [
+      "SK_GAMMA_APPLY_TO_A8",
+      "SK_GAMMA_EXPONENT=2.2",
+      "SK_GAMMA_CONTRAST=0.2",
+    ]
+  }
+   else if (is_android) {
     defines += [
       "SK_GAMMA_APPLY_TO_A8",
       "SK_GAMMA_EXPONENT=1.4",
```

# GPU acceleration

``.config/chromium-flags.conf``

```
--enable-accelerated-video-decode
--enable-accelerated-mjpeg-decode
--enable-features=VaapiVideoDecoder,CanvasOopRasterization
--enable-gpu-compositing
--enable-gpu-rasterization
--use-vulkan
--ignore-gpu-blocklist
--force-dark-mode
--enable-features=WebUIDarkMode

```

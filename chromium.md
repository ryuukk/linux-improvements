Chromium passes wrong gamma correction values, and google are too retarded to fix it

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
+      "SK_GAMMA_CONTRAST=0.0",
+    ]
+  }
+   else if (is_android) {
     defines += [
       "SK_GAMMA_APPLY_TO_A8",
       "SK_GAMMA_EXPONENT=1.4",
```

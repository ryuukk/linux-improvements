For screen 1080p or lower with relatively low DPI, tiny text on dark bg will look blurry

```
export FREETYPE_PROPERTIES="cff:no-stem-darkening=0 autofitter:no-stem-darkening=0"
```

Add this to your ``~/.profile`` file, then reboot

or patch freetype

```patch
From 0000000000000000000000000000000000000000 Mon Sep 17 00:00:00 2001
From: 
Date: 
Subject: [PATCH] Force enable stem darkening

---
diff --git a/src/base/ftinit.c b/src/base/ftinit.c
index c9c71d2..588bc51 100644
--- a/src/base/ftinit.c
+++ b/src/base/ftinit.c
@@ -180,6 +180,20 @@
       if ( !*p )
         break;
     }
+
+    // cff:no-stem-darkening=0 autofitter:no-stem-darkening=0 type1:no-stem-darkening=0 t1cid:no-stem-darkening=0
+    ft_property_string_set( library,
+                          "cff",
+                          "no-stem-darkening",
+                          "0" );
+    ft_property_string_set( library,
+                          "type1",
+                          "no-stem-darkening",
+                          "0" );
+    ft_property_string_set( library,
+                          "t1cid",
+                          "no-stem-darkening",
+                          "0" );
   }
 
 #else

```

```patch
--- orig/src/base/ftlcdfil.c	2019-02-23 10:06:07.000000000 +0100
+++ mod/src/base/ftlcdfil.c	2019-03-15 23:16:20.003565521 +0100
@@ -307,15 +307,15 @@
   /* documentation in ftlcdfil.h */
 
   FT_EXPORT_DEF( FT_Error )
   FT_Library_SetLcdFilter( FT_Library    library,
                            FT_LcdFilter  filter )
   {
     static const FT_LcdFiveTapFilter  default_weights =
-                   { 0x08, 0x4d, 0x56, 0x4d, 0x08 };
+                   { 0x1f, 0x47, 0x6B, 0x47, 0x1f };
     static const FT_LcdFiveTapFilter  light_weights =
                    { 0x00, 0x55, 0x56, 0x55, 0x00 };
 
 
     if ( !library )
       return FT_THROW( Invalid_Library_Handle );
 
```


https://freetype.org/freetype2/docs/reference/ft2-properties.html#no-stem-darkening


fuck google btw



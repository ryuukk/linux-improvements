For screen 1080p or lower with relatively low DPI, tiny text on dark bg will look blurry

```
export FREETYPE_PROPERTIES="cff:no-stem-darkening=0 autofitter:no-stem-darkening=0"
```

Add this to your ``~/.profile`` file, then reboot


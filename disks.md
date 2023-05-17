# Put to sleep noisy disks when innactive

``/etc/udev/rules.d/69-hdparm.rules``

``` 
ACTION=="add", SUBSYSTEM=="block", KERNEL=="sda", RUN+="/usr/bin/hdparm -S 30 /dev/sda"
``` 

|Parameter | Description |
|----------|:-------------:|
|-B | Set the Advanced Power Management feature. Possible values are between 1 and 255, low values mean more aggressive power management and higher values mean better performance. Values from 1 to 127 permit spin-down, whereas values from 128 to 254 do not. A value of 255 completely disables the feature. |
|-S | Set the standby (spindown) timeout for the drive. The timeout specifies how long to wait in idle (with no disk activity) before turning off the motor to save power. The value of 0 disables spindown, the values from 1 to 240 specify multiples of 5 seconds and values from 241 to 251 specify multiples of 30 minutes. |
|-M | Set the Automatic Acoustic Management feature. Most modern hard disk drives have the ability to speed down the head movements to reduce their noise output. The possible value depends on the disk, some disks may not support this feature. |

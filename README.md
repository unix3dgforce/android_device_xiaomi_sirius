For building TWRP for Xiaomi MI SE

TWRP device tree for Xiaomi MI 8 SE

Xiaomi Mi MI 8 Explorer Edition was announced and released in June 2018.

## Device specifications

| Device       | Xiaomi Mi 8 SE                                      |
| -----------: | :-------------------------------------------------- |
| SoC          | Qualcomm SDM710 Snapdragon 710                      |
| CPU          | 2x2.2 GHz 360 Gold & 6x1.7 GHz Kryo 360 Silver      |
| GPU          | Adreno 630                                          |
| Memory       | 4 GB RAM or 6 GB RAM (LPDDR4X)                      |
| Shipped Android version | 8.0                                      |
| Storage      | 128GB, 64GB UFS 2.1 flash storage  				 |
| Battery      | Non-removable Li-Po 3120 mAh                    	 |
| Dimensions   | 147.3 x 73.1 x 7.5 mm                           	 |
| Display      | 2160 x 1080 (18:9), 5.88 inch                   	 |
| Rear camera 1| 12MP, f/1.9 Dual LED flash                     	 |
| Front camera | 5MP, 1-micron pixels, f/2.0 1080p 30 fps video  	 |

## Device picture

![Xiaomi Mi 8 Explorer Edition ](http://chudo.tech/wp-content/uploads/2018/05/Xiaomi-Mi-8-SE-1-2.jpg)

## Features

Works:

- ADB
- Decryption of /data
- Screen brightness settings
- Now UI is very smooth (thanks to TWRP fix 16d831bee5a660f5ac6da0d8fff2b3ec4697d663)
- Vibration on touch (see https://gerrit.omnirom.org/#/c/android_bootable_recovery/+/31021/)
- Correct screenshot color (see https://gerrit.omnirom.org/#/c/android_bootable_recovery/+/31042/)
Finally execute these:

```
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch omni_ursa-eng 
mka recoveryimage
```

To test it:

```
fastboot boot out/target/product/ursa/recovery.img
```





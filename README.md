# OrangeFox Recovery Device configuration for Motorola Moto G82 5G

## Device specification

Basic   | Spec Sheet
-------:|:------------------------
CPU     | Octa-core (2x2.2 GHz Kryo 660 Gold & 6x1.7 GHz Kryo 660 Silver)
CHIPSET | Qualcomm SM6375 Snapdragon 695 5G (6 nm)
GPU     | Adreno 619
Memory  | 6GB, 8GB
Shipped Android Version | 12
Storage | 128GB
Battery | 5000 mAh
Dimensions | 160.9 x 74.5 x 8 mm (6.33 x 2.93 x 0.31 in)
Display | AMOLED, 120Hz, 1080 x 2400 pixels, 20:9 ratio (~402 ppi density)
Rear Camera 1 | 50 MP, f/1.8 (wide), 1/2.76", 0.64µm, PDAF, OIS
Rear Camera 2 | 8 MP, f/2.2, 118˚ (ultrawide), 1/4.0", 1.12µm
Rear Camera 3 | 2 MP, f/2.4, (macro)
Front Camera | 16 MP, f/2.2, (wide), 1.0µm

![Device Picture](https://fdn2.gsmarena.com/vv/bigpic/motorola-moto-g82.jpg)

### Kernel Source
From Lineage 23.0 Rhodep

### What's working!? :D
- Touch
- Backup && Restore
- Wipe /data
- Battery && Time
- Brightness
- MicroSD Card
- Flashing zips
- MTP && USB Mode Storage
- ADB, ADB sideload, MTP, fastbootd

**Build Command**

```bash
ulimit -n 65536
export BUILD_OFOX=true
. build/envsetup.sh
lunch twrp_rhodep-eng
mka adbd bootimage
```

Thanks to
@Samw662 
@ZetLink (https://github.com/ZetLink) for base
@Orange fox
@TWRP

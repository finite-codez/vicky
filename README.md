# Android Device Tree for Motorola Moto G72 (vicky)

## Overview

This repository contains the Android device tree for the Motorola Moto G72, codenamed "vicky". It's essential for building custom ROMs, recoveries, and kernels tailored to this device.

## Device Specifications

- **Model**: Motorola Moto G72 (XT2255-3)
- **Codename**: vicky
- **Release Date**: October 3, 2022
- **Dimensions**: 160.5 x 74.4 x 7.9 mm
- **Weight**: 166 g
- **Display**: 6.6-inch P-OLED, 120Hz refresh rate
- **Chipset**: MediaTek Helio G99 (6nm)
- **CPU**: Octa-core (2x2.2 GHz Cortex-A76 & 6x2.0 GHz Cortex-A55)
- **GPU**: Mali-G57 MC2
- **RAM**: 6GB / 8GB
- **Storage**: 128GB / 256GB, expandable via microSDXC
- **Battery**: 5000mAh with 33W fast charging
- **Rear Cameras**:
  - 108 MP (wide)
  - 8 MP (ultrawide)
  - 2 MP (macro)
- **Front Camera**: 16 MP
- **Operating System**: Shipped with Android 12; upgradable to Android 13
- **Other Features**:
  - Water-repellent design
  - Fingerprint sensor (under display)
  - Stereo speakers
  - FM radio

## Repository Structure

- `Android.mk` / `Android.bp`: Build configuration files.
- `BoardConfig.mk`: Board-specific build settings.
- `device.mk`: Device-specific configurations.
- `proprietary-files.txt`: List of proprietary binaries required for the device.
- `vendor/`: Contains vendor-specific files and blobs.
- `recovery/`: Recovery-specific configurations and resources.
- `rootdir/`: Initialization scripts and configurations.

## Building Instructions

1. **Setup the Build Environment**:
   - Ensure you have a Linux-based system with the necessary packages installed.
   - Initialize the AOSP or custom ROM source tree.

2. **Clone the Device Tree**:
   ```bash
   git clone https://github.com/YourUsername/android_device_motorola_vicky.git device/motorola/vicky

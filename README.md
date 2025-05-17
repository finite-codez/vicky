# 📱 Android Device Tree for Motorola Moto G72 (vicky)

<p align="center">
  <img src="https://fdn2.gsmarena.com/vv/pics/motorola/motorola-moto-g72-1.jpg" alt="Motorola Moto G72" width="300"/>
</p>

<p align="center">
  <a href="https://www.motorola.in/smartphones-motorola-g72/p">
    <img src="https://img.shields.io/badge/Official%20Website-Motorola-blue.svg?style=for-the-badge&logo=motorola" alt="Motorola Official Website"/>
  </a>
  <a href="https://www.gsmarena.com/motorola_moto_g72-11910.php">
    <img src="https://img.shields.io/badge/GSMArena-Specs-orange.svg?style=for-the-badge&logo=android" alt="GSMArena Specs"/>
  </a>
  <a href="https://www.youtube.com/watch?v=BJsq7LjA-Io">
    <img src="https://img.shields.io/badge/YouTube-Review-red.svg?style=for-the-badge&logo=youtube" alt="YouTube Review"/>
  </a>
</p>

---

## 📖 Overview

This repository contains the Android device tree for the Motorola Moto G72, codenamed **vicky**. It's essential for building custom ROMs, recoveries, and kernels tailored to this device.

---

## 📱 Device Specifications

| Feature            | Specification                                                                 |
|--------------------|-------------------------------------------------------------------------------|
| **Model**          | Motorola Moto G72 (XT2255-3)                                                  |
| **Codename**       | vicky                                                                         |
| **Release Date**   | October 3, 2022                                                               |
| **Dimensions**     | 160.5 x 74.4 x 7.9 mm                                                         |
| **Weight**         | 166 g                                                                         |
| **Display**        | 6.6-inch P-OLED, 120Hz refresh rate                                           |
| **Chipset**        | MediaTek Helio G99 (6nm)                                                      |
| **CPU**            | Octa-core (2x2.2 GHz Cortex-A76 & 6x2.0 GHz Cortex-A55)                       |
| **GPU**            | Mali-G57 MC2                                                                  |
| **RAM**            | 6GB / 8GB                                                                     |
| **Storage**        | 128GB / 256GB, expandable via microSDXC                                       |
| **Battery**        | 5000mAh with 33W fast charging                                                |
| **Rear Cameras**   | - 108 MP (wide)  <br> - 8 MP (ultrawide)  <br> - 2 MP (macro)                 |
| **Front Camera**   | 16 MP                                                                         |
| **Operating System** | Shipped with Android 12; upgradable to Android 13                           |
| **Other Features** | - Water-repellent design  <br> - Under-display fingerprint sensor  <br> - Stereo speakers  <br> - FM radio |

---

## 📁 Repository Structure

- `Android.mk` / `Android.bp`: Build configuration files.
- `BoardConfig.mk`: Board-specific build settings.
- `device.mk`: Device-specific configurations.
- `proprietary-files.txt`: List of proprietary binaries required for the device.
- `vendor/`: Contains vendor-specific files and blobs.
- `recovery/`: Recovery-specific configurations and resources.
- `rootdir/`: Initialization scripts and configurations.

---

## 🛠️ Building Instructions

1. **Setup the Build Environment**:
   - Ensure you have a Linux-based system with the necessary packages installed.
   - Initialize the AOSP or custom ROM source tree.

2. **Clone the Device Tree**:
   ```bash
   git clone https://github.com/finite-codez/android_device_motorola_vicky.git device/motorola/vicky
   ```

3. **Clone the Kernel Source**:
   ```bash
   git clone https://github.com/finite-codez/android_kernel_motorola_vicky.git kernel/motorola/vicky
   ```

4. **Clone the Vendor Blobs**:
   ```bash
   git clone https://github.com/finite-codez/proprietary_vendor_motorola_vicky.git vendor/motorola/vicky
   ```

5. **Lunch the Build Environment**:
   ```bash
   source build/envsetup.sh
   lunch aosp_vicky-userdebug
   ```

6. **Start the Build**:
   ```bash
   make -j$(nproc)
   ```

---

## 📝 Notes

- Ensure that you have the necessary proprietary blobs extracted from your device or obtained from reliable sources.
- Always verify the compatibility of the kernel and vendor blobs with your current Android version.
- For custom recoveries like TWRP, refer to the specific recovery tree and its building instructions.

---

## 🙌 Credits

- [SebaUbuntu](https://github.com/twrpdtgen/android_device_motorola_vicky) for the initial TWRP device tree.
- [Finite-Code](https://github.com/Finite-Code/android_device_motorola_vicky) for additional device tree configurations. (basically my 1st acc)

---

## 📄 License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for details.

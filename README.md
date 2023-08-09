# Hackintosh - Opencore EFI for Asrock B660M-ITX/ac

> **This branch is particularly for macOS Sonoma beta. It will be merged to main after the version is getting into GM.**

## Changelog

- **[8/9]**: Updated to OpenCore 0.9.4 GM. [macOS Sononma beta 5](https://swcdn.apple.com/content/downloads/26/36/042-27162-A_4GKRLRWELJ/qyzyo86g692wlsewkyclfk686op47kuq5c/InstallAssistant.pkg) is released. It has changed API for WiFi therefore a new preview version of [Airportltlwm](https://github.com/OpenIntelWireless/itlwm/issues/883#issuecomment-1670749680) has to be used.
- **[8/9]**: For Bluetooth, I am using Logitech MX Anywhere 3 mouse which has to be applied by [this patch](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/pull/446) to make it work. The patch is not merged yet so I have to use the CI build from [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/actions/runs/5639869912).
- **[7/13]**: Update to OpenCore 0.9.4 beta. Intel WiFI it uses the [preview version v0.2](https://github.com/OpenIntelWireless/itlwm/issues/883#issuecomment-1625204187) which seems fully working.
- **[5/26]**: Update to OpenCore 0.9.2. Tested on macOS Ventura 13.4.
- **[4/11]**: First commit using OpenCore 0.9.1.

## Hardware

| **Component**        | **Model**                                                                              |
| -------------------- | -------------------------------------------------------------------------------------- |
| CPU                  | Intel Core i5 12400F                                                                   |
| Motherboard          | [Asrock B660M-ITX/ac](https://www.asrock.com/mb/Intel/B660M-ITXac/index.asp)           |
| RAM                  | 16GB (2 x 8GB) G.Skill @ 2666 CL15                                                     |
| GPU                  | [PowerColor Hellhound RX 6600 - 8GB](https://www.powercolor.com/product?id=1630396326) |
| OS Disk (Nvme/Sata3) | SK Hynix P31 1TB                                                                       |
| WiFi / Bluetooth     | Intel Wireless AC 9462 and Bluetooth                                                   |
| Display              | 2 x 4K (LG and BenQ EW3270) @ 60Hz                                                     |

![Sonoma](./doc/images/sonoma.png)

## BIOS Settings

Reference - [黑苹果华擎 Asrock 主板 BIOS 详细截图设置教程](https://www.bilibili.com/read/cv12293964)

### Prerequisites

In BIOS, use `F6` to swtich to `Advanced Mode`.

### OC Tweaker

- Intel Turbo Boost Max Technology 3.0: **Enabled**

### Advanced - CPU Configuration

- Intel Hyper-Threading Technology: **Enabled**
- **CFG Lock**: **Disabled**
- Intel Virtualization Technology: **Enabled**
- **Software Guard Extensions (SGX)**: **Disabled**

### Advanced - Chipset Configuration

- Primary Graphics Adapter: **PCIe**
- Above 4G Decoding: **Enabled**
- **C.A.M (Clever Access Memory)**: **Enabled**

### Advanced - Storage Configuration

- SATA Mode Selection: **AHCI**

### Advanced - USB Configuration

- Legacy USB Support: **Enabled**
- XHCI Hand-off: **Enabled**

### Advanced - ACPI Configuration

- PS/2 Keyboard S4/S5 Wakup Support: **Enabled**
- USB Keyboard/Remote Power On: **Enabled**
- USB Mouse Power On: **Enabled**

### Advanced - Trusted Computing

- Security Device Support: **Disabled**

### Advanced - Super IO Configuration

- Serial Port: **Enabled**

### Security

- **Secure Boot**: **Disabled**

### Boot

- Fast Boot: **Disabled**
- **CSM**: **Disabled**

## Reference

- [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [OpenCore Alder Lake (12th-Gen Intel) Hackintosh Guidance](https://www.reddit.com/r/hackintosh/comments/sp1zgv/opencore_alder_lake_12thgen_intel_hackintosh/)
- [Fix shutdown and restart](https://github.com/Koala166/The-TLDR-Guide-of-Fixing-Shutdown-Restart)

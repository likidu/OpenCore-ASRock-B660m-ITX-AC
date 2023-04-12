# Hackintosh - Opencore EFI for Asrock B660M-ITX/ac

**[4/11]**: First commit using OpenCore 0.9.1.

## Hardware

| **Component**        | **Model**                                                                              |
| -------------------- | -------------------------------------------------------------------------------------- |
| CPU                  | Intel Core i5 12400                                                                    |
| Motherboard          | [Asrock B660M-ITX/ac](https://www.asrock.com/mb/Intel/B660M-ITXac/index.asp)           |
| RAM                  | 16GB (2 x 8GB) GSkill @ 2666 CL15                                                      |
| GPU                  | [PowerColor Hellhound RX 6600 - 8GB](https://www.powercolor.com/product?id=1630396326) |
| OS Disk (Nvme/Sata3) | SK Hynix P31 1TB                                                                       |
| WiFi / Bluetooth     | Onboard Intel AX210 and Bluetooth                                                      |
| Display              | 2 x 4K (LG and Benq) @ 60Hz                                                            |

![Ventura](./doc/images/ventura.png)

## BIOS Settings

Reference - [黑苹果华擎 Asrock 主板 BIOS 详细截图设置教程](https://www.bilibili.com/read/cv12293964)

### Prerequisites

In BIOS, use `F6` to swtich to `Advanced Mode`.

### Disable

#### OC Tweaker

-

* Advanced
  - CPU Configuration
    - Intel Virtualization Technology: Disabled
    - Intel VT-d: Disabled
    - Execute Disable Bit: Enabled
    - Hyper-Threading: Enabled
    - Intel SpeedStep Technology: Enabled
    - Intel Turbo Boost Technology: Enabled
    - C-States: Enabled
    - Enhanced Intel SpeedStep Technology: Enabled
    - Intel Hyper-Threading Technology: Enabled
    - Intel Turbo Boost Max Technology 3.0: Enabled
    - Intel Turbo Boost Max Technology 3.0 Driver: Enabled
    - Intel Turbo Boost Max Technology 3.0 Monitor: Enabled
    - Intel Turbo Boost Max Technology 3.0 Performance Preference: Performance
    - Intel Turbo Boost Max Technology 3.0 Power Preference: Performance
    - Intel Turbo Boost Max Technology 3.0 Technology: Enabled
    - Intel Turbo Boost Technology: Enabled
    - Intel Turbo Boost Technology Driver: Enabled
    - Intel Turbo Boost Technology Monitor: Enabled
    - Intel Turbo Boost Technology Performance Preference: Performance
    - Intel Turbo Boost Technology Power Preference: Performance
    - Intel Turbo Boost Technology Technology: Enabled
    - Intel Turbo Boost Technology Technology Driver: Enabled
    - Intel Turbo Boost Technology Technology Monitor: Enabled
    - Intel Turbo Boost Technology Technology Performance Preference: Performance
    - Intel Turbo Boost Technology Technology Power Preference: Performance
    - Intel Turbo Boost Technology Technology Technology: Enabled
    - Intel Turbo Boost Technology Technology Technology Driver: Enabled
    - Intel Turbo Boost Technology Technology Technology Monitor: Enabled
    - Intel Turbo Boost Technology Technology Technology Performance Preference: Performance
    - Intel Turbo Boost Technology Technology Technology Power Preference: Performance
    - Intel Turbo Boost Technology Technology Technology Technology: Enabled
    - Intel Turbo Boost Technology Technology Technology Technology Driver: Enabled
    - Intel Turbo Boost Technology Technology Technology Technology Monitor: Enabled
    - Intel Turbo Boost Technology Technology Technology Technology Performance Preference: Performance
    - Intel Turbo Boost Technology Technology Technology Technology Power Preference: Performance
    - Intel Turbo Boost Technology Technology Technology Technology Technology: Enabled
    - Intel Turbo Boost Technology Technology Technology Technology Technology Driver: Enabled
    - Intel Turbo Boost Technology Technology Technology Technology Technology Monitor: Enabled
    - Intel Turbo Boost Technology Technology Technology Technology Technology Performance Preference: Performance
    - Intel Turbo Boost Technology Technology Technology Technology Technology Power Preference: Performance
    - Intel Turbo Boost Technology Technology Technology Technology Technology Technology: Enabled
    -

## Reference

- [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [OpenCore Alder Lake (12th-Gen Intel) Hackintosh Guidance](https://www.reddit.com/r/hackintosh/comments/sp1zgv/opencore_alder_lake_12thgen_intel_hackintosh/)

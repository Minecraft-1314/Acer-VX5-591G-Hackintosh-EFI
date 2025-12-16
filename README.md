# Acer VX5-591G 黑苹果 EFI（更新版）
（Acer VX5-591G Hackintosh EFI [Updated]）

## 📋 硬件配置（Hardware Configuration）
| 组件（Component） | 详情（Details） |
|------------------|----------------|
| 系统（OS）| Windows 11 专业版 64位<br>Windows 11 Pro 64-bit |
| CPU | Intel Core i5-7300HQ (Kaby Lake-H)<br>4核4线程 @2.50GHz<br>指令集：SSE3/SSSE3/SSE4.1/SSE4.2/AVX/AVX2 |
| 主板（Motherboard） | 品牌：KBL / 型号：Wish_KLS<br>芯片组：HM175<br>Brand: KBL / Model: Wish_KLS<br>Chipset: HM175 |
| 内存（RAM） | 8GB DDR4 2400MHz (Micron)<br>8GB DDR4 2400MHz (Micron) |
| 硬盘（Storage） | 东芝 SSD（SATA）、SSD（SATA）、闪迪USB存储<br>Toshiba SSD (SATA)、SSD (SATA)、SanDisk USB |
| 显卡（GPU） | 核显：HD 630（支持）<br>独显：GTX 1050（无驱动）<br>iGPU: HD 630 (Supported)<br>dGPU: GTX 1050 (No Driver) |
| 网卡（Network Card） | 有线：Realtek PCIe GbE（10EC-8168）<br>Wi-Fi：Broadcom 802.11ac（14E4-43B1，已适配）<br>Wired: Realtek PCIe GbE (10EC-8168)<br>Wi-Fi: Broadcom 802.11ac (14E4-43B1, Compatible) |
| 声卡（Audio） | Realtek ALC255（支持）<br>Realtek ALC255 (Supported) |

## ✅ 正常工作（Working Functions）
- 核显HD 630（显卡加速）<br>iGPU HD 630 (Graphics Acceleration)
- 声卡ALC255（音频输入/输出）<br>Audio ALC255 (Input/Output)
- SATA硬盘/USB存储（读写）<br>SATA Storage/USB Drive (Read/Write)
- CPU/内存（电源管理）<br>CPU/RAM (Power Management)
- Broadcom Wi-Fi（原生驱动）<br>Broadcom Wi-Fi (Native Driver)
- USB接口（全功能）<br>USB Ports (Full Function)

## ❌ 不正常工作（Non-Working Functions）
- NVIDIA GTX 1050<br>NVIDIA GTX 1050 (No Hackintosh Driver)
- 部分快捷键<br>Some Hotkeys (e.g. Brightness Control Needs Extra Patches)

## ⚙️ 配置信息（Configuration Info）
| 项目（Item） | 详情（Details） |
|-------------|----------------|
| OC版本（OpenCore Version） | OpenCore 0.7.x ~ 0.8.x |
| Kexts（驱动列表） | Lilu.kext、VirtualSMC.kext、WhateverGreen.kext、AppleALC.kext、AirportBrcmFixup.kext、CPUFriend.kext、RealtekRTL8111.kext |
| 支持的macOS系统（Supported macOS） | macOS 10.14 (Mojave) ~ 11 (Big Sur) |
| BIOS设置（BIOS Settings） | 安全启动：关闭；CSM：关闭；AHCI：开启<br>Secure Boot: Disabled; CSM: Disabled; AHCI: Enabled |
| 最后更新时间（Last Updated） | 2025年12月 |

## 👥 项目贡献者（Project Contributors）
- 主维护者（Maintainer）：[你的GitHub ID]
- 测试者（Testers）：黑苹果社区同机型用户<br>Black Hackintosh Community Users with Same Model

## ⭐ 支持项目（Support This Project）
如果这个EFI帮到了你，**请给项目点一个Star**！这是对我最大的鼓励~<br>
If this EFI works for you, **please give this project a Star**! It's the best support for me~

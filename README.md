# Acer VX5-591G 黑苹果 EFI（更新版）
（Acer VX5-591G Hackintosh EFI [Updated]）

## 📋 硬件配置（Hardware Configuration）
| 组件（Component） | 详情（Details） |
|------------------|----------------|
| 系统（OS）| Windows 11 专业版 64位<br>Windows 11 Pro 64-bit |
| CPU | Intel Core i5-7300HQ (Kaby Lake-H)<br>4核4线程 @2.50GHz |
| 主板（Motherboard） | 品牌：KBL / 型号：Wish_KLS / 芯片组：HM175<br>Brand: KBL / Model: Wish_KLS / Chipset: HM175 |
| 内存（RAM） | 16GB DDR4 2400MHz (Micron) |
| 硬盘（Storage） | 东芝SSD（SATA）、SSD（SATA）、闪迪USB存储、NVMe固态硬盘<br>Toshiba SSD (SATA)、SSD (SATA)、SanDisk USB、NVMe SSD |
| 显卡（GPU） | 核显：Intel HD Graphics 630<br>独显：GTX 1050<br>iGPU: Intel HD Graphics 630<br>dGPU: GTX 1050 |
| 网卡（Network Card） | 有线：Realtek RTL8111 PCIe GbE<br>Wi-Fi：Broadcom BCM4352 802.11ac<br>Wired: Realtek RTL8111 PCIe GbE<br>Wi-Fi: Broadcom BCM4352 802.11ac  |
| 声卡（Audio） | Realtek ALC255（layout-id：29）<br>Realtek ALC255 (layout-id: 29) |
| 输入设备（Input Device） | PS/2键盘/触摸板、I2C触摸设备<br>PS/2 Keyboard/Trackpad, I2C Touch Device |

## ✅ 正常工作（Working Functions）
- Intel HD Graphics 630
- Realtek ALC255
- SATA硬盘
- USB存储
- NVMe固态硬盘
- CPU
- 内存
- Broadcom BCM4352 Wi-Fi
- 蓝牙
- Realtek有线网卡
- USB接口
- PS/2键盘
- PS/2触摸板
- I2C触摸设备
- 亮度调节快捷键
<br>
- Intel HD Graphics 630
- Realtek ALC255
- SATA Storage
- USB Drive
- NVMe SSD
- CPU
- RAM
- Broadcom BCM4352 Wi-Fi
- Bluetooth
- Realtek Wired Network Card
- USB Ports
- PS/2 Keyboard
- PS/2 Trackpad
- I2C Touch Device
- Brightness Adjustment Hotkeys

## ❌ 不正常工作（Non-Working Components）
- NVIDIA GTX 1050
<br>
- NVIDIA GTX 1050

## ⚙️ 配置信息（Configuration Info）
| 项目（Item） | 详情（Details） |
|-------------|----------------|
| OC版本（OpenCore Version） | OpenCore 1.0.6 |
| ACPI补丁（ACPI Patches/SSDT） | 启用SSDT-XOSI.aml、SSDT-PLUG.aml、SSDT-EC.aml、SSDT-PNLF.aml；_OSI→XOSI、PNLF→XNLF重命名补丁 |
| SMBIOS型号（PlatformInfo） | MacBookPro14,3（MLB：C02653700J9J1JHUE，Serial：C02T1TZRHTD5） |
| NVRAM启动参数（Boot-Args） | ipc_control_port_options=0 -amfipassbeta -brcmfxbeta brcmfx-country=HK gfxrst=1 alcid=29 -wegnoegpu slide=0 kext-dev-mode=1 -wegbeta npci=0x3000 nv_disable=1 platform=ACPI serverperfmode=1 -no_compat_check igfxonln=1 igfxrpsc=1 igfxq3d=1 |
| BIOS设置（BIOS Settings） | 安全启动：关闭；CSM：关闭；AHCI：开启<br>Secure Boot: Disabled; CSM: Disabled; AHCI: Enabled |
| 支持的macOS系统（Supported macOS） | macOS 10.12.4 ~ 26（注：macOS 26 本EFI暂不支持） |
| 最后更新时间（Last Updated） | 2025年12月16日 |

## 👥 项目贡献者（Project Contributors）
- 主维护者（Maintainer）：[[你的GitHub ID](https://github.com/Minecraft-1314)]
- 测试者（Testers）：黑苹果社区同机型用户<br>Black Hackintosh Community Users with Same Model

## ⭐ 支持项目（Support This Project）
如果这个EFI帮到了你，**请给项目点一个Star**！这是对我最大的鼓励~<br>
If this EFI works for you, **please give this project a Star**! It's the best support for me~

# Acer VX5-591G 黑苹果 EFI
Acer VX5-591G Hackintosh EFI

## 📋 硬件配置（Hardware Configuration）
| 组件（Component） | 详情（Details） |
|------------------|----------------|
| 系统（OS）| Windows 11 Pro 64-bit |
| CPU | Intel Core i5-7300HQ|
| 主板（Motherboard） | KBL Wish_KLS HM175 |
| 内存（RAM） | 16GB DDR4 2400MHz |
| 硬盘（Storage） | 东芝SSD、SSD、NVMe固态硬盘<br>Toshiba SSD、SSD、NVMe SSD |
| 显卡（GPU） | Intel HD Graphics 630<br>NVIDIA GTX 1050 |
| 网卡（Network Card） | Realtek RTL8111 <br>Broadcom BCM4352（更换后的无线网卡） <br>Broadcom BCM4352 (The replaced wireless network card)  |
| 声卡（Audio） | Realtek ALC255 |
| 输入设备（Input Device） | PS/2键盘/触摸板、I2C触摸设备<br>PS/2 Keyboard/Trackpad, I2C Touch Device |

## ✅ 正常工作（Working Functions）
- Intel HD Graphics 630
- Realtek ALC255
- SATA硬盘 SATA Storage
- USB存储 USB Drive
- NVMe固态硬盘 NVMe SSD
- CPU
- 内存 RAM
- Broadcom BCM4352 Wi-Fi
- 蓝牙 Bluetooth
- USB接口 USB Ports
- PS/2键盘 PS/2 Keyboard
- PS/2触摸板 PS/2 Trackpad
- I2C触摸设备 I2C Touch Device
- HDMI
- 麦克风 Microphone

## ❌ 不正常工作（Non-Working Components）
- NVIDIA GTX 1050
- 原装无线网卡（无驱动支持）

## ⚠️ 未测试功能（Untested Components）
- 电池 Battery
- 合盖睡眠 Lid Sleep
- 内建屏幕 Built-in Display
- 亮度调节快捷键 Brightness Adjustment Hotkeys
- Realtek有线网卡 Realtek Wired Network Card
- 显示器音频输出 Display audio output

## ⚙️ 配置信息（Configuration Info）
| 项目（Item） | 详情（Details） |
|-------------|----------------|
| OC版本（OpenCore Version） | OpenCore 1.0.6 |
| SMBIOS型号（PlatformInfo） | MacBookPro14,3 |
| BIOS设置（BIOS Settings） | 安全启动：关闭；CSM：关闭；AHCI：开启<br>Secure Boot: Disabled; CSM: Disabled; AHCI: Enabled |
| 支持的macOS系统（Supported macOS） | macOS 10.12.4 ~ 26（注：macOS 26 本EFI暂不支持）<br>macOS 10.12.4 ~ 26 (Note: This EFI does not support macOS 26 temporarily) |
| 最后更新时间（Last Updated） | 2025年12月16日 |

## ❓ 常见疑问（Frequently Asked Questions）
| 问题（Question） | 回答（Answer） |
|-----------------|----------------|
| 什么时候支持macOS 26？<br>When will macOS 26 be supported? | 需等待OCLP-MOD补丁工具实现对博通网卡的适配支持后，本EFI才会同步更新适配macOS 26系统。<br>This EFI will only be updated to support macOS 26 after the OCLP-MOD patch tool achieves compatibility with Broadcom network cards. |

## 🔧 重要提醒（Important Reminders）
### 中文
1. **SMBIOS信息**：请务必使用GenSMBIOS工具生成并手动填充专属的SMBIOS信息，SMBIOS默认为空，切勿直接使用默认信息，避免系统兼容性问题（OCAT可以一键生成）。
2. **USB驱动定制**：本EFI未包含定制化的USB驱动，需根据自身设备的USB端口情况，使用USBToolBox工具手动定制USB驱动，以保证USB接口正常工作和系统稳定性。
3. **OCLP-MOD补丁**：需手动安装并应用OCLP-MOD补丁，以解决Wi-Fi功能问题。
4. **工具使用建议**：
   - 编辑`Config.plist`文件：推荐使用OCAT软件，操作更便捷且能避免配置错误。
   - 硬件补丁制作：推荐使用Hackintools工具进行显卡、声卡等硬件的补丁制作与适配。
   - 系统补丁应用：需使用OCLP-MOD补丁工具解决Wi-Fi功能问题。
5. **macOS 26安装提示**：若需要安装macOS 26系统，本EFI暂不支持，建议使用RapidEFI工具重新生成适配的EFI文件，或根据硬件配置手动进行EFI配置调整。
6. **开源工具地址**：
   - GenSMBIOS：[https://github.com/corpnewt/GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
   - OCAT：[https://github.com/ic005k/OpenCoreAuxiliaryTools](https://github.com/ic005k/OpenCoreAuxiliaryTools)
   - Hackintools：[https://github.com/headkaze/Hackintools](https://github.com/headkaze/Hackintools)
   - OCLP-MOD：[https://github.com/laobamac/OCLP-Mod](https://github.com/laobamac/OCLP-Mod))
   - USBToolBox：[https://github.com/USBToolBox/tool](https://github.com/USBToolBox/tool)
   - RapidEFI: [https://github.com/topics/rapidefi](https://github.com/topics/rapidefi)
7. **网卡相关说明**：
   - 本项目仅适配更换后的Broadcom/intel无线网卡，设备原装无线网卡在macOS系统下无驱动支持，无法使用Wi-Fi和蓝牙功能。
   - 若不想更换内置无线网卡，可直接使用USB无线网卡，大部分USB网卡在macOS系统下无需额外添加驱动（需要软件）即可正常使用。
8. **教学资源说明**：关于黑苹果安装、硬件适配、工具使用的详细教学内容，可自行在网上查找相关教程，本项目不提供具体教学服务。

### English
1. **SMBIOS Information**: Please be sure to use the GenSMBIOS tool to generate and manually fill in your own SMBIOS information. The SMBIOS is empty by default. Do not use the default information directly to avoid system compatibility issues.(OCAT can generate this with one click)
2. **USB Driver Customization**: This EFI does not include a customized USB driver. You need to manually customize the USB driver using the USBToolBox tool according to the USB port configuration of your device to ensure that the USB interface works properly and the system is stable.
3. **OCLP-MOD Patch**: The OCLP-MOD patch needs to be manually installed and applied to resolve the Wi-Fi functionality issue.
4. **Tool Usage Recommendations**:
   - Editing `Config.plist` file: It is recommended to use OCAT software, which is more convenient to operate and can avoid configuration errors.
   - Hardware Patch Making: It is recommended to use Hackintools tool for patch making and adaptation of hardware such as graphics card and sound card.
   - System Patch Application: The Wi-Fi functionality issue needs to be resolved using the OCLP-MOD patch tool.
5. **macOS 26 Installation Note**: If you need to install macOS 26 system, this EFI does not support it temporarily. It is recommended to use the RapidEFI tool to regenerate an adapted EFI file, or manually adjust the EFI configuration according to the hardware configuration.
6. **Open Source Tool Addresses**:
   - GenSMBIOS: [https://github.com/corpnewt/GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
   - OCAT: [https://github.com/ic005k/OpenCoreAuxiliaryTools](https://github.com/ic005k/OpenCoreAuxiliaryTools)
   - Hackintools: [https://github.com/headkaze/Hackintools](https://github.com/headkaze/Hackintools)
   - OCLP-MOD：[https://github.com/laobamac/OCLP-Mod](https://github.com/laobamac/OCLP-Mod))
   - USBToolBox: [https://github.com/USBToolBox/tool](https://github.com/USBToolBox/tool)
   - RapidEFI: [https://github.com/JeoJay127/RapidEFI-Tool](https://github.com/JeoJay127/RapidEFI-Tool)
7. **Network Card Related Instructions**:
   - This project only supports the replacement of Broadcom/Intel wireless network cards. The original wireless network cards of the devices do not have driver support under macOS and cannot use Wi-Fi and Bluetooth functions.
   - If you don't want to replace the built-in wireless network adapter, you can use a USB wireless network adapter directly. Most USB network adapters can be used normally on macOS without adding additional drivers (software is required).
8. **Teaching Resources Note**: For detailed tutorials on installing Hackintosh, hardware compatibility, and tool usage, please search online for relevant tutorials. This project does not provide specific teaching services.

## 👥 项目贡献者（Project Contributors）
- 主维护者（Maintainer）：[[Minecraft-1314](https://github.com/Minecraft-1314)]
- 测试者（Testers）：黑苹果社区同机型用户<br>Black Hackintosh Community Users with Same Model

## ⭐ 支持项目（Support This Project）
如果这个EFI帮到了你，**请给项目点一个Star**！这是对我最大的鼓励~<br>
If this EFI works for you, **please give this project a Star**! It's the best support for me~

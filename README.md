# **msi-b360m-mortar_i5-9400_efi**

硬件|型号
--|:---
处理器|英特尔 Core i5-9400 @ 2.90GHz 六核
主板|微星 B360M MORTAR (MS-7B23) ( B360 芯片组 )
显卡|英特尔 UHD Graphics 630 ( 128 MB / 微星 )
内存|16 GB ( 金士顿 DDR4 2666MHz )
主硬盘|西数 WDC WDS480G2G0B-00EPW0 ( 480 GB / 固态硬盘 )
声卡|瑞昱 ALC892 @ 英特尔 High Definition Audio 控制器
网卡|英特尔 Ethernet Connection  I219-V / 微星
蓝牙|bcm94360cd

- [x] 板载有线网卡 / 无线网卡 / 蓝牙

- [x] 核心显卡

- [x] 板载声卡

- [x] 睡眠

- [x] 原生电源管理

- [x] FaceTime / iMessage

- [x] 键盘 / 鼠标唤醒

- [x] 隔空投送 / 接力 / 随航

## 更新记录

### 2020-12-30

* 更新kexts到最新版本
* 更新opencore到0.7.6
* 支持12.2 Monterey

### 2020-06-26

* 更新kexts到最新版本
* 更新opencore到0.5.9

---
STTINGS\高级\PCI子系统设置\Above 4G memory/Crypto Currency mining [允许]

STTINGS\高级\内建显示配置\设置第一显卡 [PEG]*（仅同时拥有核显及独显需要手动设置）*
STTINGS\高级\内建显示配置\集显共享内存 [64M]*（如果使用拥有核显的处理器）*
STTINGS\高级\内建显示配置\集成显卡多显示器 [允许]*（如果使用拥有核显的处理器）*

STTINGS\高级\ACPI设置\电源 LED 灯 [双色]*（如果选择 [闪烁]，睡眠时电源灯将不断闪烁）*

STTINGS\高级\USB设置\XHCI Hand-off [允许]
STTINGS\高级\USB设置\传统USB支持 [允许]

STTINGS\高级\电源管理设置\ErP Ready [允许]

STTINGS\高级\Windows操作系统的配置\Windows 10 WHQL支持 [允许]*（开启为「纯」UEFI 模式，否则为「兼容」UEFI 模式，推荐设置为允许）*
STTINGS\高级\Windows操作系统的配置\MSI 快速开机 [禁止]
STTINGS\高级\Windows操作系统的配置\快速开机 [禁止]

STTINGS\高级\唤醒事件设置\唤醒事件管理 [BIOS]
STTINGS\高级\唤醒事件设置\USB设备从S3/S4/S5唤醒 [允许]

STTINGS\启动\启动NumLock状态 [关]*（macOS 默认可使用数字键盘，只有 macOS 的话推荐关闭）*
STTINGS\启动\启动模式选择 [UEFI]

OC(Overclocking)\CPU 特征\Intel 虚拟化技术 [允许]*（必须）*
OC(Overclocking)\CPU 特征\Intel VT-D 技术 [禁止]*（必须）*
OC(Overclocking)\CPU 特征\CFG锁定 [禁止]*（必须）*

---

说明：本EFI文件是给予基于其他大佬提供打EFI文件修改，但是使用的显卡、CPU等部分硬件不一样无法直接使用，我又做了部分修改，以适配自己的配置

>https://github.com/GeQ1an/MSI-B360M-MORTAR-HACKINTOSH-OPENCORE-EFI

- 开机自动进入MacOS，如果要进入Windows，在开机bios的引导项中添加windows选项(可以使用easyuefi或者老毛桃PE中自带了UEFI开机项的管理工具)，开机按F11/F2(每家主板不太一样，根据实际情况来)选择进入windows系统

- ***clover版本请切换到clover分支***
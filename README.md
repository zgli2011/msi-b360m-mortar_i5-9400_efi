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

- 支持MacOS 10.15.X
- opencore 0.5.7
- 开机自动进入MacOS，如果要进入Windows，在开机bios的引导项中添加windows选项(可以使用easyuefi或者老毛桃PE中自带了UEFI开机项的管理工具)，开机按F11/F2(每家主板不太一样，根据实际情况来)选择进入windows系统
- ***clover版本请切换到clover分支***
---
说明：本EFI文件是给予基于其他大佬提供打EFI文件修改，但是使用的显卡、CPU等部分硬件不一样无法直接使用，我又做了部分修改，以适配自己的配置
>https://github.com/GeQ1an/MSI-B360M-MORTAR-HACKINTOSH-OPENCORE-EFI
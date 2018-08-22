## USBBootFiles
 * 说明：
        USB启动盘。只是使用grub4dos，refind等引导工具，不是自己编写新的工具。
        所以，所有引导工具版权归原作者所有。
 * BootLoader:

```
grub4dos : 在mbr+bios下使用。
refind   : 在gpt+uefi下使用，mbr+gpt也可以通过设置使用。
clover   : 用于(黑)苹果使用。
```

---
## 文件结构

```
├── autorun.inf                        : 更改u盘图标文件
├── boot
│   └── grub                           : grub4dos相关文件
│       ├── bg.bmp                     : 背景图片文件
│       ├── hotkey                     : 热键
│       ├── imgs                       : 镜像文件
│       ├──*.lst                       : 菜单设置文件
│       ├── MenuSetting                : 菜单配置文件
│       ├── SISO                       : SISO工具模块
│       └── srs                        : 驱动文件
├── cake.ico                           : u盘图标文件
├── EFI
│   ├── boot
│   │   ├── drivers_x64                : 驱动
│   │   ├── refind.conf                : 配置文件
│   │   ├── refind_x64.efi             : efi启动文件
│   │   └── styles                     : 主题
│   ├── CLOVER                         : CLOVER启动
│   └── tools                          : efi工具
├── grldr, grldr.mbr, grub.exe         : grub4dos启动文件
└── menu.lst                           : grub4dos菜单文件
```

## 常用工具

 - [BootICE：启动管理工具](http://www.ipauly.com/)
 - [DiskGenius：分区工具](http://www.diskgenius.cn/)
 - [gparted：分区工具(Linux)](https://gparted.org/)
 - [OSFMount：挂载工具](https://www.osforensics.com/tools/mount-disk-images.html)
 - [WinNTSetup：Windows系统安装工具](http://www.winntsetup.com)
 - [rEFInd：引导软件](http://www.rodsbooks.com/refind/)
 - [grub4dos：引导软件](http://grub4dos.chenall.net/)

---
## 常见问题
 - bios没有启动项
    重设bios。

 - 以UEFI方式安装其他系统
    将系统镜像解压到硬盘，在refind中添加相应启动项，启动参数参考镜像中的引导。

 - 安装Windows时或者进入PE后，无法读取SSD
    使用AHCI模式，或者使用Intel RST驱动。

---
## Contributors
 * yehuohan, yehuohan@gmail.com, 550034086@qq.com


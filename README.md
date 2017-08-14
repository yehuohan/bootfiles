# USBBootFiles
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
# 文件结构

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
│       ├── srs                        : 驱动文件
├── cake.ico                           : u盘图标文件
├── EFI
│   ├── boot
│   │   ├── drivers_x64                : 驱动
│   │   ├── refind.conf                : 配置文件
│   │   ├── refind_x64.efi             : efi启动文件
│   │   └── styles                     : 主题
│   ├── CLOVER                         : CLOVER启动
│   ├── tools                          : efi工具
├── grldr, grldr.mbr, grub.exe         : grub4dos启动文件
└── menu.lst                           : grub4dos菜单文件
```


---
# 常见问题
 * bios没有启动项
    重设bios。
 
 * 以UEFI方式安装其他系统
    将系统镜像解释到硬盘，在refind中添加相应启动项，启动参数参考镜像中的引导。


---
# Contributors
 * yehuohan, yehuohan@gmail.com, 550034086@qq.com


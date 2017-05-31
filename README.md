# USBBootFiles
 * brief:
		USB boot files with grub4dos, refind and winly.
        I just use boot loader but NOT create new boot loader.
        So, all copyright of boot loaders belong to their author.   
 * bootloadr:

```
grub4dos : used in mbr + bios
refind   : used in gpt + uefi. (mbr + uefi is ok in someway)
winly    : used in both mbr + bios and gpt + uefi.
clover   : used in mac. (google or baidu for more)
```

---
# Files

```
├── autorun.inf                        : USB icon config file
├── boot
│   └── grub                           : grub4dos files
│       ├── bg.bmp                     : background picture
│       ├── font.hex                   : font
│       ├── hotkey                     : hotkey
│       ├── imgs                       : images
│       ├──*.lst                       : boot menu list
│       ├── MenuSetting                : menu set file
│       ├── SISO                       : SISO module
│       ├── srs                        : drivers
├── cake.ico                           : USB icon
├── EFI
│   ├── boot
│   │   ├── drivers_x64                : drivers
│   │   ├── fonts                      : font files
│   │   ├── icons                      : icons for menu
│   │   ├── refind.conf                : efi config file
│   │   ├── refind_x64.efi             : efi boot file
│   │   └── styles                     : themes files
│   ├── CLOVER                         : clover boot files
│   ├── tools                          : efi tools
│   ├── winly                          : winly efi files
│   └── xorboot                        : xorboot boot files
├── grldr, grldr.mbr, grub.exe         : grub4dos boot files
├── memdisk                            : winly map file
├── menu.lst                           : grub4dos menu list
├── winly                              : winly config and themes
│   ├── themes                         : theme files
│   ├── unicode.pf2                    : font file
│   └── winly.cfg                      : config file
├── winly.iso,  winlyldr, winlyldr.mbr : winly boot files
```


---
# FAQ
 * Set default option to bios if there is no boot items.


---
# Contributors
 * yehuohan, <yehuohan@gmail.com>


---
# ChangeLog
## 20170527 - v1.2.1
 - make file-tree bautiful

## 20170315 - v1.2
 * Fix tree content with tree command.

## 20170313 - v1.1
 * Fix tree in readme
 
## 20170313 - v1.0
 * Create USBBootFiles git.


---

---


# USBBootFiles
 * 说明：   
        USB启动盘。只是使用grub4dos，refind等引导工具，不是自己编写新的工具。
        所以，所有引导工具版权归原作者所有。
 * BootLoader:

```
grub4dos : 在mbr+bios下使用。
refind   : 在gpt+uefi下使用，mbr+gpt也可以通过设置使用。
winly    : 在mbr+bios和gpt+uefi均使用。
clover   : 用于(黑)苹果使用。
```

---
# 文件结构

```
├── autorun.inf                        : 更改u盘图标文件
├── boot
│   └── grub                           : grub4dos相关文件
│       ├── bg.bmp                     : 背景图片文件
│       ├── font.hex
│       ├── hotkey                     : 热键
│       ├── imgs                       : 镜像文件
│       ├──*.lst                       : 菜单设置文件
│       ├── MenuSetting                : 菜单配置文件
│       ├── SISO                       : SISO工具模块
│       ├── srs                        : 驱动文件
├── cake.ico                           : u盘图标文件
├── EFI
│   ├── boot
│   │   ├── drivers_x64
│   │   ├── fonts
│   │   ├── icons
│   │   ├── refind.conf                : 配置文件
│   │   ├── refind_x64.efi             : efi启动文件
│   │   └── styles                     : 主题
│   ├── CLOVER                         : CLOVER启动
│   ├── tools                          : efi工具
│   ├── winly                          : winly的efi启动
│   └── xorboot                        : xorboot启动
├── grldr, grldr.mbr, grub.exe         : grub4dos启动文件
├── memdisk                            : winly镜像仿真工具
├── menu.lst                           : grub4dos菜单文件
├── winly                              : winly相关文件
│   ├── themes
│   ├── unicode.pf2
│   └── winly.cfg                      : 配置文件
├── winly.iso,  winlyldr, winlyldr.mbr : winly启动文件
```


---
# 常见问题
 * 如果bios没有启动项，重设bios。


---
# Contributors
 * yehuohna, <yehuohan@gmail.com>


---
# 日志
## 20170527 - v1.2.1
 * 让文件列表显示整齐

## 20170315 - v1.2
 * 利用tree命生成目录

## 20170313 - v1.1
 * 修改目录树
 
## 20170313 - v1.0
 * 创建USBBootFiles仓库

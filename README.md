# USBBootFiles
 * brief:
        USB boot files with grub4dos, refind and winly.
        I just use boot loader but NOT create new boot loader.
        So, all copyright of boot loaders belong to their author.   
 * bootloadr:
        grub4dos:used in mbr + bios
        refind:  used in gpt + uefi. (mbr + uefi is ok in someway)
        winly:   used in both mbr + bios and gpt + uefi.
        clover:  used in mac. (google or baidu for more)

 * Author: 
        yehuohna, <yehuohan@gmail.com>


---
# Files
/boot
    /grub/  							---grub4dos files
		  /imgs							---images
		  /src							---drivers
		  /font.hex						---font
		  /hotkey						---hotkey
		  /MenuSetting					---menu set file
		  /SISO							---SISO module
		  /splashimage.lzma				---background picture
		  /*.lst						---boot menu list
/EFI
    /boot/
		 /drivers						---drivers
		 /fonts							---font files
		 /icons							---icons for menu
		 /styles						---themes files
		 /refind_x64.efi				---efi boot file
		 /refind.conf					---efi config file
	/tool/								---efi tools
	/winly/								---winly efi files
	/xorboot/							---xorboot boot files
    /CLOVER/                            ---clover boot files
/winly/      							---winly config and themes
	  /themes							---theme files
	  /winly.cfg						---config file
      /unicode.pf2                      ---font file
/grldr, grldr.mbr, grldr.exe			---grub4dos boot files
/menu.lst								---grub4dos menu list
/memdisk								---winly map file
/winlyldr, winlyldr.bmr, winly.iso		---winly boot files
/cake.ico 							    ---USB icon
/autorun.inf							---USB icon config file


---
# Issues 
 * Set default option to bios if there is no boot items.


---
# Log
## 20170313 - v1.0
 * Create USBBootFiles git.


---

---


# USBBootFiles
 * 说明：   
        USB启动盘。只是使用grub4dos，refind等引导工具，不是自己编写新的工具。
        所以，所有引导工具版权归原作者所有。
 * BootLoader:
        grub4dos:在mbr+bios下使用。
        refind:  在gpt+uefi下使用，mbr+gpt也可以通过设置使用。
        winly:   在mbr+bios和gpt+uefi均使用。
        clover:  用于(黑)苹果使用。

 * Author:
         yehuohna, <yehuohan@gmail.com>


---
# 文件结构
/boot
    /grub/  							---grub4dos相关文件
		  /imgs							---镜像文件
		  /src							---驱动文件
		  /font.hex						---字体
		  /hotkey						---热键
		  /menuset						---菜单设置文件
		  /SISO							---SISO工具模块
		  /splashimage.lzma				---背景图片文件	  
		  /*.lst						---菜单配置文件
/EFI
    /boot/   							---refind文件启动文件
		 /drivers						---驱动
		 /fonts							---安体
		 /icons							---图标
		 /styles						---主题
		 /refind_x64.efi				---efi启动文件
		 /refind.conf					---配置文件
	/tool/								---efi工具
	/winly/								---winly的efi启动	 
	/xorboot/							---xorboot启动
    /CLOVER/                            ---CLOVER启动
/winly/      							---winly相关文件
	  /themes							---主题文件夹
	  /winly.cfg						---配置文件
      /unicode.pf2                      ---安体文件
/grldr, grldr.mbr, grldr.exe			---grub4dos启动文件
/menu.lst								---grub4dos菜单文件
/memdisk								---winly镜像仿真工具
/winlyldr, winlyldr.bmr, winly.iso		---winly启动文件
/cake.ico 							    ---u盘图标文件
/autorun.inf							---更改u盘图标文件	


---
# 问题
 * 如果bios没有启动项，重设bios。

---
# 日志
## 20170313 - v1.0
 * 创建USBBootFiles仓库

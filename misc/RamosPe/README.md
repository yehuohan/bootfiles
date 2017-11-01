
# RamosPe

用于启动Ramos、Pe、安装Windows的模板。支持Bios和UEFI，替换或添加相应的wim和sdi文件即可，或者自己修改BCD文件，修改wim和sdi文件名。

 - /winosbootmgr
```
    * config : /boot/bcd
    * load   : /boot/*.wim + /boot/*.sdi
```

 - /EFI/boot/winosbootx64.efi
```
    * config : /EFI/Microsoft/Boot/bcd
    * load   : /boot/*.wim + /boot/*.sdi
```

 - /boot/.wim & .sdi
```
    * pe64.win & peboot.sdi        : windows PE5.1_x64
    * ramosx86.win & winosboot.sdi : windows 8.1 RamOs_x86
    * boot81.win & winosboot.sdi   : windows 8.1 setup
    * boot10.win & winosboot.sdi   : windows 10 setup
```

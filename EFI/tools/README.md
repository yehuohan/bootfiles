
## List

 - KonBootDxeX64: 32/x64,无需密码直接进入WIN8系统
 - shell: the EFI shell (requires external program; see rEFInd documentation for details)
 - memtest: the memtest86 program, in EFI/tools, EFI/memtest86, EFI/memtest, EFI/tools/memtest86, or EFI/tools/memtest
 - gptsync: the (dangerous) gptsync.efi utility (requires external program; see rEFInd documentation for details)
 - gdisk: the gdisk partitioning program
 - apple_recovery: boots the Apple Recovery HD partition, if present
 - windows_recovery: boots an OEM Windows recovery tool, if present (see also the windows_recovery_files option)
 - mok_tool: makes available the Machine Owner Key (MOK) maintenance tool, MokManager.efi, used on Secure Boot systems
 - csr_rotate: adjusts Apple System Integrity Protection (SIP) policy. Requires "csr_values" to be set.
 - about: an "about this program" option
 - exit: a tag to exit from rEFInd
 - shutdown: shuts down the computer (a bug causes this to reboot many UEFI systems)
 - reboot: a tag to reboot the computer
 - firmware: a tag to reboot the computer into the firmware's user interface (ignored on older computers)
 - netboot: launch the ipxe.efi tool for network (PXE) booting

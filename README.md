# dumpnavi
This program is used to modify Acura/Honda navigation systems by dumping and modifying system files contained on the DVD.

This fork adds support for ROMOFFSET, needed to extract the Windows CE system image (at least on navigation units such as 07-08 TL).  
While it could probably automatically detect the offset, this simply attempts ROMOFFSET=0 (used on the navigation software image, e.g. 09Touch2.bin), and if that fails, attempts ROMOFFSET=-0x07FCE000 (used on the WinCE software image, e.g. 09Touch.bin)

            INIT - initramfs of YaIniT
=======================================================

This repository contains the actually used version of
the initramfs folder, used to generate the initrd file,
to place together with the YaIniT kernel into the folder
wherefrom you want to have invoked the system start by your bootloader.


CHANGES:
=========

2016-01-07:

Solved issue with the new graphic driver stack. Specifying nomon should 
work to let systemd load correctly the graphic driver. 

Introduced a working nobt (no bluetooth) for the case that some 
kernel configuration should hang at wireless initiation. 
nowlan or nowifi should work as well.

Also new is the possibility to say noserial at the kernelcommandline to
not superfluously load any RS-232 (8250) or other classical serial drivers. 

2016-01-02:

- Added support for disk labels, that contain several blanks

- Added simple support for GPT (GUUID Partition Tables)

- Restructuration: new file blockdevice-functions for blockdev operations

- A lots of corrections and accelerative simplifications



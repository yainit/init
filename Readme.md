            INIT - initramfs of YaIniT
=======================================================

This repository contains the actually used version of
the initramfs folder, used to generate the initrd file,
to place together with the YaIniT kernel into the folder
wherefrom you want to have invoked the system start by your bootloader.


CHANGES:
=========

2016-01-04:

It took a bit of time to find out that the new AMDGPU driver needs to be
blacklisted and the commandline parameters nomon and nosound have to be added.
So finally here is the new init script set!

2016-01-02:

- Added support for disk labels, that contain several blanks

- Added simple support for GPT (GUUID Partition Tables)

- Restructuration: new file blockdevice-functions for blockdev operations

- A lots of corrections and accelerative simplifications



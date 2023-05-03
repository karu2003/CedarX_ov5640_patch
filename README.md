# CedarX + ov5640
build mith armbian build https://github.com/armbian/build
copy patch to userpatches\kernel\archive\sunxi-6.2

./compile.sh build BOARD=bananapim2zero BRANCH=edge BUILD_DESKTOP=no BUILD_MINIMAL=no KERNEL_CONFIGURE=yes RELEASE=sid

Enable Driver in
> Device Drivers > Staging drivers > Media staging drivers
[*]   Allwinner sunXi family Video Devices
<*>     Allwinner CedarX Video Engine Driver
<*>     Allwinner CedarX Ion Driver 

Config "DMA Contiguous Memory Allocator"
> Library routines
-*- DMA Contiguous Memory Allocator
*** Default contiguous memory area size: ***
(96)  Size in Mega Bytes
Selected region size (Use mega bytes value only)  --->


# useful links
https://github.com/peteallenm/cedar

https://github.com/aodzip/cedar

https://github.com/peteallenm/gst-plugin-cedar-cs

https://github.com/FREEWING-JP/OrangePi_CedarX

https://github.com/PaserTech-Hardware/cedar

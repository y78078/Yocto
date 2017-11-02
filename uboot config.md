# uboot

## uboot countdown

### clean uboot 
bitbake -c clean u-boot-imx

bitbake -c cleansstate u-boot-imx

bitbake u-boot-imx

### edit uboot config

build/tmp/work/imx6dlsabresd-poky-lunux-gnueabi/u-boot-imx/2016.03-r0/git/include/configs/mx6_common.h

-#define CONFIG_BOOTDELAY	3

+#define CONFIG_BOOTDELAY	0

### rebuild
bitbake -f -c compile u-boot-imx

bitbake -f -c build u-boot-imx

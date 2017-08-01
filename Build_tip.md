# Note: Freescale 3.14.28-1.0.1 release kernel & u-boot
一開始的工作應該是改這兩個kernel & u-boot東西 還要看一下怎樣做才正確

Bitbake 的 Recipes

./yocto_3.14.28-1.0.1/sources/meta-fsl-bsp-release/imx/meta-fsl-arm/recipes-bsp/u-boot/u-boot-imx_2014.04.bb
./yocto_3.14.28-1.0.1/sources/meta-fsl-bsp-release/imx/meta-fsl-arm/recipes-kernel/linux/linux-imx_3.14.28.bb
透過 Recipes 會把Source code 解壓縮或是透過git clone/pull 的方式弄到下面對應的build folder 裡面去，主要看 Recipes 的寫法

./yocto_3.14.28-1.01/build/tmp/work/imx6dlsabresd-poky-linux-gnueabi/u-boot-imx/2014.04-r0/git
./yocto_3.14.28-1.01/build/tmp/work/imx6dlsabresd-poky-linux-gnueabi/linux-imx/3.14.28-r0/git

## rootfs打包
tar jcvf rootfs.tar.bz2 *

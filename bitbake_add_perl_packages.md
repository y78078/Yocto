# perl

## Can't locate foobar.pm in @INC errors.
https://stackoverflow.com/questions/20037681/how-can-i-install-missing-perl-modules-on-an-embedded-system

## Add perl common packages 
### path: ${build-dir}/souces/poxy/meta/poky/meta/recipes-devtools/perl/perl_5.22.1.bb
find PACKAGES = "perl-XXXX" add here 

## “Can't locate loadable object for module Tie::Hash::NamedCapture in @INC” even after installing the module?
### put to target cross compile path:
### /opt/fsl-imx-fb/4.1.33-7ulp_beta/sysroots/x86_64-pokysdk-linux/usr/lib/perl/5.22.1/NamedCapture.so

### get from build path:
### /home/scout/nxp/build_qt5/tmp/work/x86_64-nativesdk-pokysdk-linux/nativesdk-perl/5.22.1-r0/packages-split/nativesdk-perl-module-tie-hash-namedcapture/opt/fsl-imx-fb/4.1.33-7ulp_beta/sysroots/x86_64-pokysdk-linux/usr/lib/perl/5.22.1/auto/Tie/Hash/NamedCapture/NamedCapture.so

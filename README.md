android_device_lge_e400
=======================

TWRP ==> device tree for l3 (e400)

pls note this is only twrp specific device tree

CyanogenMod 11 device configuration for L3 (e400)

http://forum.xda-developers.com/showthread.php?t=2700336

How to build:
=============

Initialize repo:

repo init -u git://github.com/SlimRoms/platform_manifest.git -b kk4.4-caf
curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.github.com/sooorajjj/android_device_lge_e400/blob/master/manifest_lge_e400.xml
curl -L -o .repo/local_manifests/manifest_lge_e400.xml -O -L https://raw.github.com/sooorajjj/android_device_lge_e400/blob/master/manifest_lge_e400.xml
repo sync
Compile:

 source build/envsetup.sh
 breakfast e400
 brunch e400

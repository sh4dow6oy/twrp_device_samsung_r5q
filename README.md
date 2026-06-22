# TWRP Device Tree for Samsung Galaxy S10 Lite

## Notes

FBEv1 decryption might or might not work and only if no password was set

## Kernel Source

Prebuilt from latest Android 13 firmware (G770FXXS9HXA1)

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/LumiPlayground/twrp_device_samsung_r5q.git -b android-12.1 device/samsung/r5q
```

3. To build:

```bash
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch twrp_r5q-eng
mka recoveryimage
```

# TWRP device tree for Nothing Phone 3 sm8735

## Supported devices

- Nothing Phone 3

## Build it yourself?

```shell
mkdir twrp && cd twrp
repo init --depth=1 -u https://github.com/TWRP-Test/platform_manifest_twrp_aosp.git -b twrp-16.0
repo sync
git clone --depth=1 https://github.com/DrBrown28/twrp_device_Meteoid_sm8735.git
```

```shell
source build/envsetup.sh
lunch twrp_Metroid
make recoveryimage
```

If there is no error, recovery.img will be found in `out/target/product/sm87xx/recovery.img`

## Features

Works:

- [X] ADB
- [X] Display
- [X] Decryption
- [X] Fastbootd
- [X] Flashing
- [X] MTP
- [X] Sideload
- [X] Touch
- [X] USB OTG
- [X] Vibrator

## To use it:

```shell
fastboot flash recovery recovery.img
```

or

```shell
fastboot flash recovery_a recovery.img
fastboot flash recovery_b recovery.img
```

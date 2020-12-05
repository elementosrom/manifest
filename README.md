Current version: vanadium

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg?style=flat)](https://github.com/elementCAF/manifest)

# ElementOS
Pure AOSP ROM with all Pixel exclusives apps and goodies, built with SystemUIGoogle to bring Pixel devices a new life

### Building ElementOS for your device
Init and sync the repo
```
repo init -u https://github.com/elementosrom/manifest -b eleven
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Export and build
```
. build/envsetup.sh

lunch aosp_(chipset_id)-userdebug
mka bacon
```

### Adding dependencies
You must add all dependencies for your device including kernel and its headers, device tree, common tree and product/vendor files

Current version: uranium

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg?style=flat)](https://github.com/brainrepoCAF/manifest) [![OTA Status](https://img.shields.io/badge/OTA%20Status-disabled-red.svg?style=flat)](https://github.com/brainrepoCAF/manifest)

![BrainRepo](https://github.com/brainrepoCAF/docs/raw/uranium/images/BRBanner.png)
# CodeAurora Forum // BrainRepo
### Based on CAF
Faster and lighter than AOSP based repos. Come and build with CAF!

---------
- Latest CAF Intel Driver: May 9, 2020
- Latest CAF Common Driver: May 9, 2020
- Latest AOSP legacy update repo: October 3, 2019

# Building CAF for your device
Init and sync the repo
```
repo init -u https://github.com/brainrepoCAF/manifest -b uranium
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Export and build
```
. build/envsetup.sh

lunch caf_(chipset_id)-eng
mka bacon
```

# Adding dependencies
You must add all dependencies for your chipset including kernel and its headers, chipset tree, common processor tree and product/vendor files

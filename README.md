Current version: uranium

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg?style=flat)](https://github.com/brainrepoCAF/manifest)

# BrainRepo
### Building CAF for your device
Init and sync the repo
```
repo init -u https://github.com/brainrepoCAF/manifest -b uranium
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Export and build
```
. build/envsetup.sh

lunch caf_(chipset_id)-userdebug
mka ottapackage
```

### Adding dependencies
You must add all dependencies for your chipset including kernel and its headers, chipset tree, common processor tree and product/vendor files

### Driver
- Latest CAF Qcom Driver: Aug 24, 2020
- Latest CAF Common Driver: July 29, 2020
- Latest AOSP legacy update repo: July 13, 2029

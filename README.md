![Banner](https://github.com/ElementOSROM/tools/blob/master/images/manifest_rev1.png?raw=true)

Current version: arsenic

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

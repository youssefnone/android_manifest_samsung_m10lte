# crDroid

### How to build ###

```bash
# Create dirs
$ mkdir crdroid ; cd crdroid

# Init repo
$ repo init --depth=1 -u git://github.com/crdroidandroid/android.git -b 10.0

# Clone my local repo
$ git clone https://github.com/youssefnone/android_manifest_samsung_m10lte.git -b crdroid .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && lunch lineage_m10lte-eng && mka clean && mka api-stubs-docs && mka hiddenapi-lists-docs && mka system-api-stubs-docs && mka test-api-stubs-docs && mka bacon -j`nproc`
```

## Credits
thanks @Astrako 2019
@youssefnone @2022
thanks @samsungexynos7870 team

## Contact
Telegram support group: https://t.me/joinchat/D1Jk_VbieGBXOWZt2y8O7A

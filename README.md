# crDroid

### How to build ###

```bash
# Create dirs
$ mkdir crdroid ; cd crdroid

# Init repo
$ repo init --depth=1 -u https://github.com/crdroidandroid/android.git -b 10.0

# Clone my local repo
$ git clone https://github.com/youssefnone/android_manifest_samsung_m10lte.git -b crdroid-10 .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && lunch lineage_m10lte-user && mka clean && mka api-stubs-docs && mka hiddenapi-lists-docs && mka system-api-stubs-docs && mka test-api-stubs-docs && mka bacon -j`nproc`
```

## Credits
2019 @Astrako
2023 @AndVer

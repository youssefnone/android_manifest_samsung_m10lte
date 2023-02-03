# ResurrectionRemix 8

### How to build ###

```bash
# Create dirs
$ mkdir rr8 ; cd rr8

# Init repo
$ repo init --depth=1 -u https://github.com/ResurrectionRemix/platform_manifest.git -b Q

# Clone our local repo
$ git clone https://github.com/samsungexynos7870/android_manifest_samsung_m10lte.git -b rr-8 .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && mka clean && brunch rr_a3y17lte-user
```

## Credits
2019 @Astrako, POSP, LOS and RR branches kept up to date by @Sap1k
2023 @youssefnone

# Pixel Extended #
<img src="https://imgur.com/likQDEZ.png">

### Sync ###

```bash

# Initialize local repository
repo init --depth=1 -u git://github.com/PixelExtended/manifest -b ten-plus

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```


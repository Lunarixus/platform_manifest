## Prepare your environment ##
[Set up your build environment](https://source.android.com/setup/build/initializing)
## Init the source ##
```bash
repo init -u https://github.com/hentaiOS/platform_manifest -b Rika
```
## Sync the memes ##
```bash
repo sync --force-sync -j$(nproc --all)
```
## Get the bread ##
```bash
. build/envsetup.sh
lunch hentai_<device>-user
make otapackage -j$(nproc --all)
```

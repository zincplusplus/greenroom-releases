# greenroom-releases
Greenroom for Mac: notarized builds. Turns an iPhone into a background-replacing camera.

## Install or update

Quits Greenroom, downloads the latest release, replaces the app in /Applications, prints the version and opens it.

```bash
pkill -x Greenroom; cd /tmp && rm -f Greenroom.zip && curl -sLO https://github.com/zincplusplus/greenroom-releases/releases/latest/download/Greenroom.zip && rm -rf /Applications/Greenroom.app && ditto -x -k Greenroom.zip /Applications && defaults read /Applications/Greenroom.app/Contents/Info.plist CFBundleShortVersionString && open /Applications/Greenroom.app
```

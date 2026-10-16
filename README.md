# Mac Porter Lab updates

[Download the latest Mac Porter Lab release](https://github.com/well13514/mac-porter-updates/releases/latest)

This repository hosts signed app downloads and the update feed. App source code, game files, Wine runtimes, signing keys and local release metadata are not published here.

## Install once, then update in the app

1. Open the latest release and download its `Mac-Porter-Lab-*.zip` file.
2. Unzip it and put **Mac Porter Lab.app** in Applications or another writable folder.
3. Open the app. Future versions are checked daily by default. Use **Settings → Check Now** or **Mac Porter Lab → Check for Updates…** to check manually. Automatic checks can be disabled in Settings.

The older Mac Porter 0.9 app has no configured updater, so it cannot install the first updater-enabled build automatically. Mac Porter Lab uses a separate data folder and does not automatically import the older app's games or Wine prefixes.

## Requirements and signing

- Apple silicon Mac, macOS 26 or later.
- A separately configured Wine runtime and game installations.
- The current personal Lab build is not Developer ID signed or notarized. macOS may require first-run approval under Privacy & Security.
- Sparkle verifies the signed update feed and downloaded archive against the public key embedded in the app before installing updates.

Update feed: [appcast.xml](https://github.com/well13514/mac-porter-updates/releases/latest/download/appcast.xml)

Versioned download assets are immutable. Every update receives an increasing build number.

<a href="https://apps.obtainium.imranr.dev/redirect?r=obtainium://app/%7B%22id%22%3A%22479970496%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2FGlazedBelmont%2Fes-de-android-custom-systems%22%2C%22author%22%3A%22GlazedBelmont%22%2C%22name%22%3A%22es-de-android-custom-systems%22%2C%22preferredApkIndex%22%3A0%2C%22additionalSettings%22%3A%22%7B%5C%22includePrereleases%5C%22%3Afalse%2C%5C%22fallbackToOlderReleases%5C%22%3Atrue%2C%5C%22filterReleaseTitlesByRegEx%5C%22%3A%5C%22%5C%22%2C%5C%22filterReleaseNotesByRegEx%5C%22%3A%5C%22%5C%22%2C%5C%22verifyLatestTag%5C%22%3Atrue%2C%5C%22dontSortReleasesList%5C%22%3Afalse%2C%5C%22useLatestAssetDateAsReleaseDate%5C%22%3Afalse%2C%5C%22releaseTitleAsVersion%5C%22%3Afalse%2C%5C%22trackOnly%5C%22%3Atrue%2C%5C%22versionExtractionRegEx%5C%22%3A%5C%22%5C%22%2C%5C%22matchGroupToUse%5C%22%3A%5C%22%5C%22%2C%5C%22versionDetection%5C%22%3Atrue%2C%5C%22releaseDateAsVersion%5C%22%3Afalse%2C%5C%22useVersionCodeAsOSVersion%5C%22%3Afalse%2C%5C%22apkFilterRegEx%5C%22%3A%5C%22%5C%22%2C%5C%22invertAPKFilter%5C%22%3Afalse%2C%5C%22autoApkFilterByArch%5C%22%3Atrue%2C%5C%22appName%5C%22%3A%5C%22ES-DE%20XMLs%5C%22%2C%5C%22shizukuPretendToBeGooglePlay%5C%22%3Afalse%2C%5C%22allowInsecure%5C%22%3Afalse%2C%5C%22exemptFromBackgroundUpdates%5C%22%3Afalse%2C%5C%22skipUpdateNotifications%5C%22%3Afalse%2C%5C%22about%5C%22%3A%5C%22%5C%22%2C%5C%22refreshBeforeDownload%5C%22%3Afalse%7D%22%2C%22overrideSource%22%3Anull%7D"> <img src="https://github.com/ImranR98/Obtainium/blob/main/assets/graphics/badge_obtainium.png?raw=true" alt="Click me to add the repository to Obtainium!" width="256">

Those 2 XMLs will add in the following systems
- Gameboy Hacks (`gbh`)
- Gameboy Color Hacks (`gbch`)
- Gameboy Advance Hacks (`gbah`)
- Genesis Hacks (`genh`)
- NES Hacks (`nesh`)
- SNES Hacks (`snesh`)
- Switch (`switch`)
- Microsoft Xbox (`xbox`), including [HakuX-Mali](https://github.com/Wannamingo/HakuX-Mali)

They are to be placed in `ES-DE/custom_systems` (Download them and copy/paste them into that directory, make sure you don't have them end as `.txt`, they _have_ to be `.xml`).
After adding the custom system files make sure to fully close ES-DE and restart it for the custom system files to load (not just rescan roms).

## HakuX-Mali (Microsoft Xbox)

Install [HakuX-Mali 1.0 or later](https://github.com/Wannamingo/HakuX-Mali/releases/latest), open it once, complete setup and grant it access to the same `ROMs/xbox` folder used by ES-DE. This is required because the launch command passes the game path using the emulator's `rom_path` extra; ES-DE's folder access does not grant access to the emulator.

After installing these XML files and restarting ES-DE, select **HakuX-Mali (Standalone)** for **xbox** under **Alternative Emulators**. The existing X1 BOX, hakuX and Xenra alternatives are retained.

ISO/XISO images can be launched directly. For an extracted game, keep all its files together and launch its `default.xbe`, for example `ROMs/xbox/Manhunt/default.xbe`. Other XBE filenames are not standalone launch targets in HakuX-Mali.

The published APK uses package `com.rfandango.haku_x.debug`, despite being an optimized release build. Its activity is `com.rfandango.haku_x.LauncherActivity` (without `.debug`), so the find rule uses the full activity name.


Why the hacks folders? I come from JelOS and these folders were present, art-book-next-es-de also has support for those now. **This also means other themes may just display a generic image for hacks**


# I am not affiliated with ES-DE in any way apart from being a supporter.

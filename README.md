# TP Browser updates

New versions of **TP Browser** are published here. Installed copies of the app check this repository by themselves and offer to update, so nobody has to reinstall by hand.

| Platform | Latest version info | Download |
| --- | --- | --- |
| Android 7.0+ | [`android/latest.json`](android/latest.json) | `android/TP-Browser-<version>.apk` |
| Mac | [`mac/latest.json`](mac/latest.json) | `mac/tp-browser-mac-<version>.zip` (TP Browser's own code; the app downloads it by itself) |
| iPhone / iPad (iOS 15+) | [`ios/latest.json`](ios/latest.json) | `ios/TP-Browser-<version>.ipa` · AltStore/SideStore source: [`ios/altstore.json`](ios/altstore.json) |

To install TP Browser on a new phone, download the newest APK from the `android` folder, open it, and allow installing from your browser or Files app.

Every APK is signed with the same TP Browser key. Android refuses an update signed with any other key, and the app also checks each download's SHA-256 against `latest.json` before installing.

On the Mac, TP Browser 2.2.1 and newer check `mac/latest.json` every few hours, download the new code in the background, check its SHA-256, and switch to it when you restart. The Chromium engine stays the same; a version that needs a newer engine (`minElectron`) asks you to run the builder again instead. TP AI's key is never part of these files.

**iPhone and iPad:** TP Browser isn't on the App Store, so it's sideloaded with your Apple ID. In **SideStore** or **AltStore**, add the source `https://raw.githubusercontent.com/kornchapattonpoon/tp-browser-updates/main/ios/altstore.json` and install TP Browser from it; they keep it signed and offer new versions of the app. Or install `ios/TP-Browser-<version>.ipa` with **Sideloadly**. TP's screens also update themselves inside the app (`ios/latest.json`, verified with SHA-256).

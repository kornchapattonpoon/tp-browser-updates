# TP Browser updates

New versions of **TP Browser** are published here. Installed copies of the app check this repository by themselves and offer to update, so nobody has to reinstall by hand.

| Platform | Latest version info | Download |
| --- | --- | --- |
| Android 7.0+ | [`android/latest.json`](android/latest.json) | `android/TP-Browser-<version>.apk` |

To install TP Browser on a new phone, download the newest APK from the `android` folder, open it, and allow installing from your browser or Files app.

Every APK is signed with the same TP Browser key. Android refuses an update signed with any other key, and the app also checks each download's SHA-256 against `latest.json` before installing.

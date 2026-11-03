# Install and update Viyam

## Requirements

- Android 7.0 (API 24) or later.
- SMS access is only needed for optional bank-alert features.
- No Viyam account or server setup is needed.

## First installation

1. Open the [official Releases page](https://github.com/atheeqrc/Viyam-Releases/releases).
2. Select a release and download its `.apk` asset. GitHub's Source code archives contain this documentation, not an installable app.
3. Open the downloaded APK. Android may ask you to allow installations from the browser or file manager you are using.
4. Allow that source if you choose to proceed, then install Viyam. You can turn that source permission off afterward.
5. Open Viyam and follow the setup guide. SMS permission is optional.

After installing, you can turn off the browser or file manager's permission to install unknown apps. That source permission is separate from Play Protect scanning.

## Google Play Protect

Viyam is distributed as an APK outside Google Play and requests optional SMS permissions. Play Protect may recommend a scan, show a warning, or block installation. Google describes sensitive-permission blocks for apps downloaded through browsers, messaging apps or file managers as a financial-fraud protection measure. This is different from a warning that specifically identifies an app as harmful. Read the actual message shown on your device. [Google Play Protect warning types](https://support.google.com/work/android/answer/15162069?hl=en).

- **Scan recommended:** keep Play Protect enabled and accept the scan if offered. Review its result before proceeding.
- **Installation blocked or harmful-app warning:** stop the installation and report the exact message through [GitHub Issues](https://github.com/atheeqrc/Viyam-Releases/issues). Include the Android version, Viyam version and a screenshot with personal information removed. The publisher can investigate and appeal an incorrect classification through Google's official process.
- **Signing conflict or incompatible update:** keep your existing installation if you need its data; see Updates below. This is separate from a Play Protect decision.

Google recommends keeping Play Protect enabled. Turning it off reduces protection and does not certify an APK as safe or guarantee installation. This online guide provides current installation guidance alongside the illustrated PDF. [Google's Play Protect guidance](https://support.google.com/accounts/answer/2812853?hl=en) and [app verification appeals](https://support.google.com/android/answer/2992033?hl=en).

Download only from this repository's official Releases page. A verified APK signature and matching SHA-256 checksum establish signing identity and file integrity; they do not establish Google Play approval or prove that a warning is incorrect.

## Updates

Download the next APK from this repository and install it over the existing release. An in-place update requires a compatible application ID and signing certificate and an acceptable version code. Viyam does not currently include an automatic updater.

**If Android reports a signing conflict, do not uninstall Viyam or clear storage if you need its records.** Updates must use a compatible signing certificate. The app currently has no export/restore feature; uninstalling would erase its ledger. Keep your existing installation and report the update problem through GitHub Issues without sharing personal financial information.

The public release uses application ID `com.atheeq.viyam`.

## Verify a download

Each published APK should have a matching entry in the release's `SHA256SUMS.txt`. On Windows PowerShell:

```powershell
Get-FileHash .\Viyam-1.0.0-beta.1.apk -Algorithm SHA256
```

On macOS:

```sh
shasum -a 256 Viyam-1.0.0-beta.1.apk
```

On Linux:

```sh
sha256sum Viyam-1.0.0-beta.1.apk
```

Compare the complete value with `SHA256SUMS.txt` from the same official release. A matching hash confirms file equality, not an independent security audit.

The signing certificate fingerprint is recorded in the release notes. Developers can inspect the APK using Android SDK `apksigner verify --print-certs`.

## Data retention

Keep Viyam installed if you need its history. Uninstalling or clearing storage deletes local records. Android backup is disabled and there is no cloud synchronization, export or restore in this beta.

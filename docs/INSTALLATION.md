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

Android or Play Protect may show prompts for apps distributed outside Google Play. Review them before deciding whether to install. This distribution does not establish Google Play approval.

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

# Viyam 1.0.1

Released 21 November 2026. Android compatibility update.

## Fixed

- Fixes a launch failure on Android 10 in the initial 1.0.0 beta release.
- Retains the existing features and local data format. This is the recommended release for new installations and updates.

## Release details

- APK: `Viyam-1.0.1-beta.1.apk` (5233580 bytes).
- In-app version: `1.0.1`, version code `3`.
- Application ID: `com.atheeq.viyam`; minimum Android 7.0 / API 24.
- Uses the same signing certificate as the previous public release.
- Startup, manual setup, sample expense classification and data persistence after an in-place reinstall were verified on Android 10. The 198 JVM unit tests pass; release lint reports zero errors and 46 warnings.

APK SHA-256:

```text
01d7c9bd18c68f5116c8905fc13e13ab0f65c73b22df34ab4302a28b07ea6b14
```

Signing certificate SHA-256:

```text
37f94ac501b56829b16a93d5e178532c97d7c1a05db43145dea3580760935316
```

## Installation and data

Install this APK over a compatible existing public release. Debug builds use a different signing key and may not accept this update. Do not uninstall or clear storage if you need saved records: this version has no export or restore.

See the [installation guide](INSTALLATION.md), [privacy notice](PRIVACY.md), [user guide](USER_GUIDE.md) and [known limitations](LIMITATIONS.md). The illustrated PDF describes the 1.0.0 feature set; this patch fixes startup compatibility.

Review recorded amounts and classifications against your records.

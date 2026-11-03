# Viyam 1.0.0 beta 1

Released 3 November 2026. First public evaluation build.

## Included

- Manual income/expense entry and optional bank SMS tracking.
- Multiple accounts, custom categories, monthly and category budgets.
- Review of original approved-sender messages and unsupported alerts.
- Confirmation workflows for own-account transfers, investments and reversals.
- Reports by account, period, category and merchant.
- Local storage, optional SMS access, and no Internet permission.

See the [user guide](USER_GUIDE.md), [privacy notice](PRIVACY.md) and [known limitations](LIMITATIONS.md).

## Build and verification

- APK: `Viyam-1.0.0-beta.1.apk` (3,092,278 bytes).
- In-app version: `1.0.0`, version code `2`; the GitHub release marks this build as beta.
- Application ID: `com.atheeq.viyam`; minimum Android 7.0 / API 24; target API 37.
- Release build completed successfully with release optimization enabled.
- Configured JVM unit-test suite: 198 tests, zero failures/errors (Gradle verified cached results were up to date).
- Release lint: zero errors, 46 warnings covering dependency updates, unused resources, drawing allocations, tooling constructors, API style and localization.
- APK Signature Scheme v2 and v3 verification passed; ZIP alignment verification passed.
- **Installation and runtime testing of this signed release have not been completed.** The available emulator configuration is missing its Android system image. No release was installed on the developer's everyday phone.

APK SHA-256:

```text
864d0df6821a266378259b96a2a203f8d5b796172ed3650e7460dce1dee17fc7
```

Signing certificate SHA-256:

```text
37f94ac501b56829b16a93d5e178532c97d7c1a05db43145dea3580760935316
```

## Before installing

This beta has no export or restore. Uninstalling or clearing storage deletes its ledger. If an existing debug build has a different signing key, **do not uninstall it to bypass a signing conflict**. Keep the existing installation and arrange a data-preserving migration before switching. See [installation and updates](INSTALLATION.md).

Amounts and reports require user review and are not bank-reconciled balances. Test with sample data before relying on this beta for your records.

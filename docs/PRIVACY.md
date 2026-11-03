# Privacy notice

Effective date: 3 November 2026. Applies to the initial Viyam Android beta distributed here.

## Data kept on your phone

Viyam stores your account names and purposes, budgets, categories, sender selections, merchant preferences, transactions and review decisions in Android app-private storage. Approved-sender SMS records can include original message text, extracted amounts, sender identifiers, receipt times and source hashes used for duplicate detection.

The application requests no Internet permission and does not upload this data. The current app includes no analytics or advertising SDK. Android backup is disabled. App-private storage provides Android's application isolation; Viyam does not claim additional database encryption or protection against an unlocked, compromised or rooted device.

## Optional SMS access

If you grant SMS access, sender discovery scans incoming SMS conversations for financial language to suggest senders. This discovery is independent of the tracking start date. Sender discovery does not create ledger entries or retain message bodies. When you explicitly open a latest-message preview, the app displays that sender's latest received message transiently.

You approve the senders to track. Historical imports retain messages from approved senders within the selected date range. New messages from approved senders are saved from the configured tracking date onward. **All approved-sender messages may be retained, including OTPs, promotions and service notices.** Unsupported messages remain available for review rather than automatically changing financial totals.

Original messages remain stored with records. Ignoring a message excludes it from review and accounting but retains its text and source ID so re-import does not revive it. Stopping a sender's tracking does not erase existing history. Revoking SMS permission in Android settings stops further SMS access but does not delete records already stored.

## Permissions

| Permission | Purpose |
| --- | --- |
| Read SMS (`READ_SMS`) | Discover senders, preview messages and import selected history. Optional. |
| Receive SMS (`RECEIVE_SMS`) | Track new alerts from approved senders after the tracking boundary. Optional. |
| Notifications (`POST_NOTIFICATIONS`) | Show transaction review notifications; requested on Android 13 and later. |

No Contacts or Internet permission is requested. Manual transaction entry works without SMS access.

## Notifications

Transaction notifications may show financial details such as a merchant and amount. Android's notification and lock-screen settings control their visibility. Unsupported-message notifications use a generic review action without displaying the raw message or OTP. Disable notifications or hide sensitive lock-screen content in Android settings if needed.

## Removal and backups

Uninstalling Viyam or clearing its app storage deletes its local data. **This is irreversible in the current beta:** no export, restore or cloud sync is provided. If an update fails, keep the existing installation if you need its records.

## GitHub and feedback

This notice describes the app. GitHub hosts this repository and downloads under its own policies. Issues and screenshots you post publicly are visible to others. Submit only fictional or fully redacted examples. For privacy questions about the app, open an issue without including personal financial information.

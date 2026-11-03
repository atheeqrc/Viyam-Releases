# Beta limitations

- Currency and transaction parsing focus on LKR / Rs alerts. Sender selection does not guarantee that every message format can be parsed.
- Regression examples include selected HNB INTERNET and account-credit formats, COMBANK card purchases/cancellations, and Amana CEFTS, POS and reversal formats. This is example coverage, not certification or universal support for those banks.
- OTPs, failed payments, statements and ambiguous messages are excluded from automatic money movements. All approved-sender messages may still be stored for review.
- Unrecognized messages require review, explicit transaction recording or ignoring.
- Amounts can reflect an authorization or approximation rather than final settlement. Validate against your records.
- Accounts and reports describe recorded transactions, not live balances. No bank connection, reconciliation or investment market pricing is provided.
- Sender identifiers can be spoofed and are not proof of bank identity. Approval only controls which senders Viyam tracks.
- Existing history may be incomplete, especially after changing the tracking date or sender selection. Automatic duplicate detection is based on source identifiers and available timestamps, not bank reconciliation.
- Android permission settings and device background restrictions can affect live SMS capture and notifications. Review history if alerts appear to be missing.
- No export, restore, cloud synchronization or automatic app updater is included. Uninstalling or clearing storage deletes the ledger.
- A public release key can differ from an existing debug installation's key. Do not uninstall a debug build to bypass a signing conflict if you need its data.

Beta builds may contain bugs. Report reproducible issues using synthetic examples at [GitHub Issues](https://github.com/atheeqrc/Viyam-Releases/issues).

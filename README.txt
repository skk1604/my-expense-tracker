EXPENSE TRACKER V2 — IPHONE INSTALLATION AND ALERT IMPORT

1. Unzip this archive using the iPhone Files app.
2. Upload ALL files in this folder to the ROOT of your existing GitHub repository my-expense-tracker, replacing the previous files. Keep the exact same GitHub Pages URL so IndexedDB records remain accessible.
3. GitHub repository > Settings > Pages > Deploy from branch main / root. Wait for deployment.
4. Open the published URL in Safari; refresh and launch from Home Screen. If the old UI persists, close and reopen while online.
5. In bank app or Gmail, COPY the text of a transaction alert (never copy OTPs, passwords, full card details). Open the app > Import bank alert / Gmail message > Paste clipboard or paste into the field > Extract transaction > Review > Approve & save.
6. Optional Shortcut: create a Shortcut with Receive Text from Share Sheet, URL Encode the provided text, combine your EXACT GitHub Pages URL + #import= + encoded text, then Open URLs. This is user-initiated, not background monitoring. Test with a fake transaction. Avoid sharing sensitive content in URL fragments; fragments can be visible in browser history or other device contexts. Copy/paste is preferred.
7. Gmail: Copy transaction alert text from Gmail into the app. This version does NOT connect to Gmail or read messages in the background. Truly automatic Gmail polling needs a separate online service, explicit Google OAuth permissions, and secure server-side design. Do not place API tokens in GitHub Pages code.
8. iOS does NOT give an ordinary PWA unrestricted access to bank push notifications. Do not rely on notification auto-capture.
9. Import parsing is best-effort. Some bank messages have multiple amounts (e.g. balances) and may be parsed incorrectly. Review each proposed transaction. Duplicate detection uses date, currency, amount, debit/credit, source and description; it can miss near-duplicates.
10. Export JSON backup regularly to iPhone Files / iCloud Drive. JSON restore replaces all records. Avoid uploading backups to public GitHub repositories.
11. All transaction data is in local IndexedDB. GitHub Pages hosts only application code. Bank alert text is not transmitted to a server by this app.

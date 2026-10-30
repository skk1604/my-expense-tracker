MY DAILY EXPENSE TRACKER — iPHONE SETUP

1. Upload ALL files from this folder together to a static HTTPS host (for example GitHub Pages, Netlify or Cloudflare Pages). The folder must contain index.html, sw.js, manifest.webmanifest and both PNG icons.
2. Open the published HTTPS URL in Safari on your iPhone while online.
3. Tap Share (square with up arrow) > Add to Home Screen > Add. Launch the Expenses icon.
4. Open once while online to cache the app; thereafter it can work offline.
5. Enter transactions, select SGD/INR/USD, debit or credit, and source. Filter by date, currency, account or search.
6. BACKUP: Tap Export JSON. In iOS download/share UI choose Save to Files (On My iPhone or iCloud Drive). Make backups regularly, especially before browser cleanup or phone replacement.
7. RESTORE: Tap Import JSON, choose the saved backup, confirm replacement. Import REPLACES existing records.
8. CSV export is for Excel/Numbers and is not a restorable backup.

PRIVACY: Transactions are stored in IndexedDB on the device under the published website's origin. The app itself makes no financial-data network requests. Static hosting serves application code only. Browser data can be deleted by iOS or the user. This is not a guaranteed permanent file in Files; JSON export is your portable backup. Do not use private browsing. A different website URL/origin will have a separate database.

NOTE: This ZIP is source files, not an App Store app. iOS does not reliably install an offline PWA directly from a local file:/// URL.

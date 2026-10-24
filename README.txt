DBZ Vault Android 0.6 — portfolio interface

CameraX scanner, gallery scanning and seven-star icon are retained.
Automatic pricing: exact English Masters, Fusion World and Panini matches from TCGplayer Market via TCGCSV, converted from USD to AUD using Frankfurter reference rates. The provider snapshot is updated daily by GitHub Actions. The app checks its own hosted feed at most daily and retains the last working prices offline.

Manual vintage prices remain unchanged and take priority. Unsupported cards, alternate artwork without an exact mapping, graded/played/damaged holdings and Japanese cards are not assigned English base-card prices. Market references are not guaranteed resale prices. Source dates, FX dates and matched product links are shown in card details.

The optional catalogue audit and artwork-index panels are hidden; the native camera scanner does not depend on them. Native Android file saving is available for collection backup and CSV exports. Status-bar insets prevent the header from overlapping phone indicators.

Build source: DBZ-Vault-GitHub-APK-Build-Ready.zip. Package com.dbzvault.collector.nativescan, version code 6. Uses the same development signing key as versions 0.4 and 0.5, allowing installation as an update without removing collection data.

Validation: JavaScript syntax and scanner tests; price-matching and manual-override tests; Android lint and APK compilation. Physical-device verification is still required for updated Android UI integrations.

Data sources: https://tcgcsv.com/ and https://frankfurter.dev/
GitHub Actions restores the existing PUBLIC DEVELOPMENT-ONLY signing key from repository history. The source upload excludes signing-key files. This is not a production credential.

Portfolio layout: dark dashboard with large AUD value, most-valuable cards, recent additions, cleaner card details and central scanner navigation. Portfolio history records the priced portion of the collection on days the app is opened. New history begins when priced cards are added; past values and gains are never fabricated. Vintage manual pricing is retained.

DBZ Vault Android 0.9 — one-button binder price updates

CameraX scanner, gallery scanning and seven-star icon are retained.
Automatic pricing: exact English Masters, Fusion World and Panini matches from TCGplayer Market via TCGCSV, converted from USD to AUD using Frankfurter reference rates. The provider snapshot is updated daily by GitHub Actions. The app checks its own hosted feed at most daily and retains the last working prices offline.

Manual vintage prices remain unchanged and take priority. Unsupported cards, alternate artwork without an exact mapping, graded/played/damaged holdings and Japanese cards are not assigned English base-card prices. Market references are not guaranteed resale prices. Source dates, FX dates and matched product links are shown in card details.

The optional catalogue audit and artwork-index panels are hidden; the native camera scanner does not depend on them. Native Android file saving is available for collection backup and CSV exports. Status-bar insets prevent the header from overlapping phone indicators.

Build source: DBZ-Vault-GitHub-APK-Build-Ready.zip. Package com.dbzvault.collector.nativescan, version code 9. Uses the same development signing key as versions 0.4 and 0.5, allowing installation as an update without removing collection data.

Validation: JavaScript syntax and scanner tests; price-matching and manual-override tests; Android lint and APK compilation. Physical-device verification is still required for updated Android UI integrations.

Data sources: https://tcgcsv.com/ and https://frankfurter.dev/
GitHub Actions restores the existing PUBLIC DEVELOPMENT-ONLY signing key from repository history. The source upload excludes signing-key files. This is not a production credential.

Portfolio layout: dark dashboard with large AUD value, most-valuable cards, recent additions, cleaner card details and central scanner navigation. Portfolio history records the priced portion of the collection on days the app is opened. New history begins when priced cards are added; past values and gains are never fabricated. Vintage manual pricing is retained.

0.7 changes: recognise combined front/back leader names and Parallel Foil market subtypes, preserve exact set and artwork checks. Existing binder entries receive matching prices without re-scanning. New matcher versions rebuild the feed even when the source date is unchanged. Updated bundled prices supersede old cached matching data. Manual values keep priority. WebView now sits inside an inset-aware native container, keeping fixed headers, bottom navigation, card dialogs and scanner controls clear of status/navigation bars and keyboard.

Automatic adding: a unique exact printed-number match of 100 saves one card immediately, with Undo. Repeated scans do not increment quantity. Ambiguous codes and corrected/fuzzy readings remain suggestions. New entries keep finish Not set until Normal/Foil is chosen; this moves the entry instead of adding a second card. No reflective finish is inferred from glare. Reviewed original BT2-001 and BT1-031 standard holographic products can use their exact TCGplayer Normal-labelled product prices, explicitly disclosed in source details; no general cross-finish fallback is used.

0.8: native scanner uses its original window startup path, with scanner-specific safe-area padding installed after setContentView. The WebView retains its separate safe-area container. Android instrumentation checks open/reopen the camera and open it through the scan tab and JavaScript bridge.

0.9: replace the expanded price research queue with Update card prices. A user-initiated update bypasses the automatic daily check interval and retrieves the latest hosted snapshot, automatically revaluing matching binder entries and portfolio totals. Shows a compact result rather than individual research rows. Manual values remain authoritative; unsupported/vintage cards remain manual. Offline failures retain the last valid prices and show a clear status. Scanner startup fix and Android camera launch tests are retained.

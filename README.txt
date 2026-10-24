DBZ Vault Android 0.4 — native scanning

Build source is DBZ-Vault-GitHub-APK-Build-Ready.zip; GitHub Actions extracts this project before building.
CameraX uses a lifecycle-bound compatible preview instead of WebView video.
Bundled ML Kit reads printed alphanumeric card numbers offline, including codes on Japanese cards. Automatic capture requires the same unique catalogue number in two consecutive readings. Tap to focus; Read now and Gallery also work without an automatic match.
Full-photo OCR falls back to focused corner crops. Review artwork/variants and choose Normal/Foil before saving. Unlisted vintage cards can still be saved manually; artwork alone is not a guaranteed identification.
Package ID: com.dbzvault.collector.nativescan. Version code 4. This installs alongside the earlier Camera Fix APK, preserving that app and its binder. Existing collections do not transfer automatically. The new app uses the same HTTPS origin and storage format for compatible backups.

Validation: node tests/recognition.test.cjs; gradle testDebugUnitTest lintDebug assembleDebug.
Physical-device camera and foil/glare checks are still required.

Signing: debug.keystore is a PUBLIC DEVELOPMENT-ONLY Android debug key, used for consistent signatures in future personal test builds. It is not a production credential. Earlier APKs used ephemeral runner keys. This app uses a separate package ID, so there is no need to uninstall them. Never use this key for a production release.

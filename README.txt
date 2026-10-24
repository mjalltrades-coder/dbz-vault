DBZ Vault Android 0.4 — native scanning

Build source is DBZ-Vault-GitHub-APK-Build-Ready.zip; GitHub Actions extracts this project before building.
CameraX uses a lifecycle-bound compatible preview instead of WebView video.
Bundled ML Kit reads printed alphanumeric card numbers offline, including codes on Japanese cards. Automatic capture requires the same unique catalogue number in two consecutive readings. Tap to focus; Read now and Gallery also work without an automatic match.
Full-photo OCR falls back to focused corner crops. Review artwork/variants and choose Normal/Foil before saving. Unlisted vintage cards can still be saved manually; artwork alone is not a guaranteed identification.
Package ID, HTTPS app origin and binder storage keys are unchanged from the Camera Fix build. Version code 4.

Validation: node tests/recognition.test.cjs; gradle testDebugUnitTest lintDebug assembleDebug.
Physical-device camera and foil/glare checks are still required.

Signing: debug.keystore is a PUBLIC DEVELOPMENT-ONLY Android debug key, used for consistent signatures in future personal test builds. It is not a production credential. Earlier APKs built with ephemeral runner keys may need a binder backup and uninstall before this APK installs. Never use this key for a production release.

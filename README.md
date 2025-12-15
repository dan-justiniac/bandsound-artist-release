# bandsound-artist-preview

BandSound Artist — macOS preview (unsigned, unnotarized)

https://github.com/dan-justiniac/bandsound-artist-release/releases/tag/0.1.0-preview

How to install (Universal build: Apple Silicon + Intel)
1) Open the DMG (BandSound-Artist-0.1.0-preview-mac-universal.dmg).
2) Drag “BandSound Artist” into Applications.
3) First launch: macOS will warn because the app is unsigned.
   - Right-click the app in Applications → Open → confirm.
   - If blocked, go to System Settings → Privacy & Security → “Open Anyway”.
4) Future launches will open normally.

Using the ZIP instead
- Unzip the .zip, move “BandSound Artist” to Applications, then perform step 3 once.

Build info
- Version: 0.1.0-preview
- Codesign/notarization: none (expected for preview)
- Targets produced by “npm run compile” on macOS: DMG and ZIP (universal)

Support checks
- If the app doesn’t start: make sure you completed the right-click Open once.
- If Gatekeeper still blocks: re-download, ensure the DMG/ZIP isn’t quarantined (xattr -dr com.apple.quarantine “BandSound Artist.app”).

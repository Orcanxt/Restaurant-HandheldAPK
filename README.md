# Orca Restaurant POS — Handheld update channel

Release builds of the OrcaPOS Android handheld (`com.orca.pos`), and the manifest the app reads
to update itself.

- **Manifest (fixed URL every tablet polls):**
  `https://github.com/Orcanxt/Restaurant-HandheldAPK/releases/download/manifest/handheld-manifest.json`
- **Builds:** one release per version (`vX.Y.Z`), asset `OrcaPOS-Handheld-X.Y.Z.apk`.

Each APK is signed with the Orca handheld release key
(certificate SHA-256 `A8:1A:D4:75:1E:5F:04:04:5E:6F:9D:1C:B6:F7:A1:F2:D8:09:00:0C:40:4C:E7:8F:35:A4:2F:1E:8B:78:4A:0E`),
and the manifest carries each APK's SHA-256, which the app checks before installing.

First install on a tablet: download the latest APK from Releases and open it.
From 1.1.0 on, the app offers new versions itself (Login → ⚙ → Check for updates).

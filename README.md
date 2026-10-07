# AsyBrain HUB releases

Public Windows and Linux installers and signed updates for AsyBrain HUB.

Download versioned packages from [Releases](https://github.com/asygames/asybrain-hub-releases/releases).

- Windows: per-user NSIS installer, with signed automatic updates.
- Linux: AppImage for signed automatic updates; DEB and RPM packages for manual package updates.
- Automatic check intervals: 5 minutes, 1, 6, 12, 24 hours or a custom interval.
- Updates wait until active work is finished.

All builds, tests and release verification run locally. GitHub Actions is not used.
The stable updater endpoint is `releases/download/stable/latest.json`. It is published only after the referenced versioned artifacts are verified from GitHub.

Signatures authenticate the downloaded package and bind it to the announced version. Windows Authenticode is separate from updater signatures.

# PowerModeManager Releases

Official distribution repository for PowerModeManager. Product details and English and Korean installation guidance are published on the [official website](https://powermodeapp.github.io/).

## Latest release

The stable release is **1.0.0 (Build 8)**. It provides a signed and notarized DMG for Apple Silicon Macs, with macOS 15 as the minimum version. There is no public beta download, and ZIP distribution is not offered.

## Install with Homebrew

Homebrew Casks from non-official taps require explicit trust. Add the tap, trust only the PowerModeManager Cask, then install:

```sh
brew tap powermodeapp/tap
brew trust --cask powermodeapp/tap/powermodemanager
brew install --cask powermodemanager
```

Upgrade with `brew upgrade --cask powermodemanager`. See the [Homebrew tap](https://github.com/powermodeapp/homebrew-tap) for details.

## Install from the DMG

Download [PowerModeManager.dmg](https://github.com/powermodeapp/PowerModeManager-Releases/releases/latest/download/PowerModeManager.dmg) and its [SHA-256 checksum](https://github.com/powermodeapp/PowerModeManager-Releases/releases/latest/download/PowerModeManager.dmg.sha256) from the latest release. Open the DMG and move PowerModeManager to Applications.

## Supported systems and verification

The release requires Apple Silicon and macOS 15 or later. Build 8 was verified on Mac16,8 with macOS 27.0.1 (Build 26A434) and in a macOS Sequoia UTM virtual machine. Intel Macs are not supported.

Server Mode disables system sleep in its profile and may increase power use and battery drain on a laptop. Review the proposed settings, keep a MacBook connected to power while using Server Mode, and restore Normal Mode when continuous availability is no longer needed. The app does not provide battery charge limits or stop charging.

## Get help

Report a problem in [GitHub Issues](https://github.com/powermodeapp/PowerModeManager-Releases/issues) in English or Korean. Include the app version, macOS version, Mac model, and steps to reproduce. Review diagnostic data before sharing; do not attach raw diagnostics that may contain private host information.

For a suspected security vulnerability, use [private vulnerability reporting](https://github.com/powermodeapp/PowerModeManager-Releases/security/advisories/new). Do not post security details in a public issue.

## License

PowerModeManager is free under the [MIT License](LICENSE). The license permits redistribution and sale subject to its notice. The app includes the [Yams license notice](THIRD_PARTY_NOTICES/Yams-LICENSE.txt).

# CamUnlocks Support Tool - releases

Public host for the CamUnlocks Support Tool auto-updater and remote config.
The code lives in a separate private repo; only signed release artifacts and the
signed config live here.

- `config.signed.json` - the signed remote config (flagged Windows updates, a
  message, and the forced-update switch). Edit it by signing a new one in the
  code repo and committing it here. The tool reads it on launch and verifies the
  signature, so a tampered file is rejected.
- Each GitHub Release carries the installer and `latest.json`. The tool checks
  the latest release on launch and updates itself.

Everything here is Ed25519-signed by CamUnlocks. Do not edit files by hand.

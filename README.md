# LineageOS-Sado OTA metadata

This repository serves update metadata for the LineageOS-Sado builds.
The LineageOS Updater reads the root-level `<device>.json` file for the
current device.

Each file follows the LineageOS Updater response schema documented in
`packages/apps/Updater/README.md`. CI should replace the empty array with
the published build metadata after uploading an OTA package.

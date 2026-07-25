# LineageOS-Sado OTA metadata

This repository serves update metadata for the LineageOS-Sado builds.
The LineageOS Updater reads the root-level `<device>.json` file for the
current device.

Each file follows the LineageOS Updater response schema documented in
`packages/apps/Updater/README.md`. CI replaces the empty array with metadata
generated from the signed package after its SourceForge upload succeeds.

See [`example.json`](example.json) for a complete reference. The package
checksum, size, timestamp and payload offsets must never be entered manually.
The `type` and `version` fields must match `ro.lineage.releasetype` and
`ro.lineage.build.version` on the target build.

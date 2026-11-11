# onn7core 36020962

Development and recovery notes for the **2026 onn. 7 Core**, model **36020962** (`onn7core`).

This repository preserves a known-good technical baseline and provides a clean workspace for future Android development, recovery work, scripts, notes, and reproducible experiments.

## Known device baseline

- Device: onn. 7 Core
- Model: `36020962`
- Codename: `onn7core`
- Android: 16
- SDK: 36
- Build: `BP2A.250605.031.A3`
- Incremental: `20260623`
- Security patch: `2026-04-05`
- Platform: MediaTek
- Partition scheme: A/B, dynamic partitions, `super`, EROFS
- Root method tested: Magisk-patched `init_boot_b`
- Magisk 30.7 was used for the original root work
- The patched `init_boot` method has been independently reported working by another owner of the same tablet/build.

## Repository purpose

This is a development/research repository, **not a factory-firmware mirror**.

Good candidates for Git:
- device notes
- partition maps
- hashes
- root/recovery procedures
- Magisk module source
- scripts and tooling
- recovery/device-tree research
- reproducible test notes

Large raw partition images, full `super.img` dumps, and complete firmware archives should stay outside normal Git history.

## Stock dump download

The full stock partition dump is hosted externally because the images are too large for normal Git history.

Dropbox:
https://www.dropbox.com/scl/fo/lh8fe5bilrdga5pjywkjr/AH6i2hRoSHvg5lB83KG9RWo?rlkey=bzus3p9h66yxeuzz72kag3sll&dl=0

Archive:
`onn7core_36020962_20260623_stock_dump.7z`

SHA-256:
`767cd7753cfd8b2a56078aa3f4e29e9d7cb9ffc9f5efb4464e5f3ab3416ae931`

This is a device-derived stock partition dump, not an official factory image or flash-all package. Verify the archive hash before using it.

## Current status

- Stock partition dump preserved separately
- Stock `init_boot_b.img` preserved
- Root working via patched `init_boot_b`
- Custom boot animation Magisk module tested
- Custom recovery work has not yet begun

## Safety

Use at your own risk. Flashing the wrong image, flashing an image to the wrong slot/partition, or using files from a different build can cause boot failure or device damage.

Verify the exact device, build, partition, slot, and hash before flashing anything.

## Project rule

Start from the known-good baseline, document each experiment, and prefer reversible changes whenever possible.

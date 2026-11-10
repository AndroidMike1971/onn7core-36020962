# Recovery research

Custom recovery work has **not started yet**.

This file is the staging area for future recovery investigation.

## Initial questions

- Which recovery architecture is appropriate for this Android 16 A/B MediaTek device?
- Is recovery embedded in boot/vendor_boot or represented separately on this build?
- What ramdisk and fstab sources are available from the preserved dump?
- What is required for decryption/data access?
- Which dynamic-partition operations are safe from recovery?
- Can partition-level wipe/format controls be exposed safely?

## Development rule

Start with read-only reconnaissance. Do not flash a recovery image until the boot chain, partition target, rollback path, and known-good stock images have been re-verified.

## Goal

Eventually produce a reproducible recovery-development path for model 36020962 without treating this repository as a firmware mirror.

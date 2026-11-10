# Device baseline

## Identity

- Device: onn. 7 Core
- Model: `36020962`
- Codename: `onn7core`
- Platform: MediaTek

## Software baseline

- Android: 16
- SDK: 36
- Build: `BP2A.250605.031.A3`
- Incremental: `20260623`
- Security patch: `2026-04-05`

## Storage / partition architecture

- A/B device
- Dynamic partitions
- `super` partition present
- EROFS used

## Known-good state

- Stock partition dump preserved separately from this Git repository.
- Stock `init_boot_b.img` preserved separately.
- Root has been achieved with a Magisk-patched `init_boot_b`.
- The patched init_boot approach has been independently reported working by another owner of the same tablet/build.

## TODO

- Re-verify exact partition list and sizes from the saved dump before adding them here.
- Record bootloader/fastboot observations from a fresh bench session.
- Record exact hardware identifiers only from live device output or preserved authoritative logs.

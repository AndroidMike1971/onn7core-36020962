# Root notes

## Verified device/build

- Device: onn. 7 Core
- Model: `36020962`
- Codename: `onn7core`
- Android: 16
- SDK: 36
- Build: `BP2A.250605.031.A3`
- Incremental: `20260623`
- Security patch: `2026-04-05`

## Verified root baseline

- Magisk version used for original root: `30.7`
- Active slot at root installation: `B`
- Patched partition: `init_boot_b`
- Device mapping: `/dev/block/mmcblk0p44`

### Stock init_boot_b.img

- Size: `8,388,608 bytes`
- SHA-256:

`be629572126caafaf6270198a916cf54bf2cf1a5e1f6e9a369428d151fcde195`

### Magisk-patched init_boot_b.img

- Size: `8,388,608 bytes`
- SHA-256:

`9e977153c56a1f045a152b0e4392ea4bf656b56f16e80b770374a569b94e54d7`

## Verified slot-B flash command

`fastboot flash init_boot_b magisk_patched_init_boot_b.img`

Do not assume another tablet is currently using slot B. Verify first:

`fastboot getvar current-slot`

## Verified rollback command

`fastboot flash init_boot_b init_boot_b.img`

`fastboot reboot`

## Root verification

`adb shell`

`su`

`id`

Verified development-device result:

`uid=0(root) gid=0(root) context=u:r:magisk:s0`

Root persisted after a normal reboot.

## Recommended public method

Prefer patching the tablet's own stock `init_boot` image with Magisk instead of blindly flashing a pre-patched image.

Always verify:

- exact model
- exact firmware/build
- active slot
- target partition
- image hash
- stock rollback image

The original full notes are preserved under `docs/source-material/` and `magisk/`.

# Verified hashes

Large firmware and partition images stay outside normal Git history. Their hashes are recorded here so locally stored or separately distributed artifacts can be verified.

## Root images

### Stock init_boot_b.img

SHA-256:

`be629572126caafaf6270198a916cf54bf2cf1a5e1f6e9a369428d151fcde195`

### Magisk-patched init_boot_b.img

SHA-256:

`9e977153c56a1f045a152b0e4392ea4bf656b56f16e80b770374a569b94e54d7`

## Stock dump archive

`onn7core_36020962_20260623_stock_dump.7z`

SHA-256:

`767cd7753cfd8b2a56078aa3f4e29e9d7cb9ffc9f5efb4464e5f3ab3416ae931`

## Full stock partition hash list

See:

`SHA256SUMS-stock-dump.txt`

That file contains hashes for the preserved boot-chain and super partition images.

## Rule

A matching filename is not enough. Verify both the exact device/build and SHA-256 before flashing.

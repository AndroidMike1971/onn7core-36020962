# Partition map

Known architecture:

- A/B slots
- Dynamic partitions
- `super` partition
- EROFS

The exact partition inventory, sizes, logical-group layout, and slot-specific details still need to be copied from the preserved device dump or re-read from the tablet.

## Rule

Do not fill this table from assumptions or from a similar MediaTek device. Use only this tablet's own output/dump.

| Partition | Slot | Type | Size | Notes |
|---|---|---|---:|---|
| `init_boot` | A/B | boot-related | TODO | Stock `init_boot_b` preserved; patched B image used for original root work |
| `super` | shared/dynamic container | dynamic | TODO | Contains logical partitions |

Additional rows: TODO after re-verification.

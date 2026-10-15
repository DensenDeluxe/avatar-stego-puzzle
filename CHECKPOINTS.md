# Checkpoints // hard edition

These are **partial seals**, not instructions. All values are lowercase hexadecimal. Each check shows only the first 8 bytes of a SHA-256 digest.

| Seal | Prefix | What it verifies |
|---|---|---|
| Glass ledger | `7453c8593fbde68c` | Your reconstruction of the Archive's full-wall fingerprint |
| Lost name | `2e770615c70b4c87` | The recovered 24-character name |
| Forged key | `ffd441e34c1a73ec` | The final 32-byte forge output |
| Station walk | `d4dc20c368fb023a` | The ordered walk, after you serialize the first twelve stations consistently |
| Oath | `747c2f7d31df85fc` | The exact ASCII oath remembered by the vault |

The crate verifies itself once you reach it. A matching prefix does not replace authenticated decryption.

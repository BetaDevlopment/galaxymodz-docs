# OrbSpawn — Security & Anti-Exploit

OrbSpawn is designed from the ground up to be exploit-proof. Every known spawner duplication and ownership bypass vector is mitigated.

---

## Exploit Mitigations

| Exploit Vector | Mitigation |
|---|---|
| **Piston Duplication** | Pistons cannot push or pull spawner blocks |
| **Explosion Duplication** | Explosions do not produce spawner item drops |
| **Egg Swap Exploit** | Mob type is locked in PDC at creation — mismatched eggs are always rejected. Null `getSpawnedType()` is handled; egg insertion is blocked if type is unknown |
| **Egg Storage Exploit** | Eggs are never stored in the spawner item PDC — the egg count cannot be duplicated via pick-up/re-place cycle |
| **Ownership Bypass** | Admin check uses the correct `orbspawn.admin` node (old bug using `spawnercontrol.admin` was fixed in v3.5) |
| **GUI Double-Delivery** | Block is removed before items are given. `ConcurrentHashMap` flag prevents concurrent duplicate delivery |
| **Pickup Spam** | Per-player cooldown (default 3s) enforced server-side |
| **Event Cancel Bypass** | `EventPriority.LOWEST` + `ignoreCancelled=false` — OrbSpawn reads data before any protection plugin can cancel or interfere |

---

*Next: [Compatibility & Limitations](compatibility.md)*

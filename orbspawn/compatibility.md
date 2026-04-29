# OrbSpawn | Compatibility & Known Limitations

## Supported Integrations

| Plugin | Role |
|---|---|
| TebexCheckout | Tebex integration for spawner delivery via donation packages |
| BuycraftX | Alternative Tebex client | both supported simultaneously |
| RoseStacker | Stacked mob compatibility |
| WildStacker | Alternative stacker | also fully supported |

> OrbSpawn supports **78 mob types** | all mobs with valid spawn eggs in the 1.21.4 API, excluding Ender Dragon and Wither.

---

## Known Limitations & Warnings

| | Details |
|---|---|
| **License Key Required** | Network call on startup. Plugin will not load if the key is absent, invalid, or the license server is unreachable. |
| **Eggs Not Stored in Items** | Intentional security design. Admins must use `extraegg` to compensate if a player loses eggs before re-fuelling. |
| **Pickup GUI Timeout** | The pickup GUI expires after 30 seconds. Timed-out pending entries are cleaned up automatically. |
| **Old Spawners (Pre-v3.5)** | Spawners placed before the entity-type lock was added lack `ENTITY_TYPE_KEY`. They fall back to `getSpawnedType()`, which returns the correct type for all normally placed spawners. |
| **1.21.4+ Required** | Plugin declares `api-version: 1.21.4`. Older 1.21.x builds may show a load warning. |
| **No-prefix Bedrock** | If a server removes the Geyser dot prefix and two players share a name, Minecraft itself prevents simultaneous login. This is a server configuration concern, not an OrbSpawn issue. |

---

*Next: [Support & Contact](support.md)*

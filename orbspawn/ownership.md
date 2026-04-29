# OrbSpawn | Ownership & Transfer

Ownership is stored in Persistent Data Container (PDC) entries on both the spawner block and the spawner item. UUID-based storage means it survives name changes, server restarts, and cross-platform play.

---

## PDC Data

| Key | Type | Stored On | Purpose |
|---|---|---|---|
| `owner_uuid` | String (UUID) | Block + Item | The owner's unique player ID |
| `owner_name` | String | Block + Item | Display name (dot-prefix stripped for Bedrock) |
| `allowed_spawner` | Byte (1) | Block + Item | Marks it as OrbSpawn-managed |
| `entity_type` | String | Block + Item | Locked mob type (prevents egg-swap exploit) |
| `egg_fuel` | Integer | Block only | Current egg count |

---

## Transfer Rules

- Player must hold the spawner item in their **main hand**
- Player must be the **registered owner** OR have `orbspawn.admin`
- Target player must be **online**
- Cannot transfer to yourself
- Item PDC is updated immediately with the new owner's UUID and name
- Both the sender and receiver receive chat confirmation

---

## Transfer Command

```
/orbspawn transfer <player>
/obs transfer <player>
```

See [Commands](commands.md) for full details.

---

*Next: [Bedrock / Geyser Support](bedrock.md)*

# OrbSpawn | How It Works: Spawner Pickup

## Trigger Methods

| Action | Required Item | Result |
|---|---|---|
| Shift + Right-Click spawner | Empty hand | Opens pickup GUI |
| Shift + Left-Click spawner | Any pickaxe | Opens pickup GUI |

---

## Pickup Flow

1. Player triggers pickup via Shift + Click
2. Event fires at `LOWEST` priority | reads spawner data before any other plugin can interfere
3. Ownership is verified | non-owners without `orbspawn.admin` are rejected
4. Cooldown is checked | player is notified if still within the cooldown window
5. GUI opens showing: mob type, location, owner name, current egg fuel count
6. **YES clicked** → spawner block is removed **first** (anti-dupe), then items are given to inventory
7. If inventory is full, all items drop at the spawner's location
8. Pickup cooldown is applied to the player

---

> **Warning**
> The block is always removed **before** items are given. This prevents duplication exploits where a player disconnects between block removal and item delivery.

---

> **Important | Egg Behaviour Change**
> Spawners no longer come with eggs bundled when given via `/cspawner`. This was changed to close a major duplication exploit. Use `/cspawner <player> <mob> extraegg <n>` if you want to give eggs alongside a spawner.

---

*Next: [How It Works | Egg Fuel](how-it-works-eggs.md)*

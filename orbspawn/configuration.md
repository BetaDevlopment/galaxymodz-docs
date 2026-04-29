# OrbSpawn | Configuration

File: `plugins/OrbSpawn/config.yml`
Apply changes with: `/orbspawn reload`

---

## Config Keys

| Key | Type | Default | Description |
|---|---|---|---|
| `license-key` | String | *(required)* | Commercial license key |
| `enabled` | Boolean | `true` | Master on/off switch |
| `block-natural-spawners` | Boolean | `true` | Lock all naturally generated spawners |
| `allow-trial-spawners` | Boolean | `true` | Allow Trial Chamber spawners |
| `allow-player-spawners` | Boolean | `true` | Allow player-placed spawners to spawn |
| `allow-tebex-spawners` | Boolean | `true` | Allow Tebex-purchased spawners |
| `block-all-dimensions` | Boolean | `true` | Block natural spawners in all dimensions |
| `disable-natural-spawner-xp` | Boolean | `true` | No XP from breaking natural spawners |
| `prevent-piston-duplication` | Boolean | `true` | Pistons cannot move spawners |
| `prevent-explosion-duplication` | Boolean | `true` | Explosions do not drop spawner items |
| `enable-pickup-gui` | Boolean | `true` | Show GUI confirmation on pickup |
| `require-pickup-permission` | Boolean | `true` | Require `orbspawn.pickup` to pick up |
| `pickup-cooldown` | Integer | `3` | Seconds between pickups per player |
| `debug` | Boolean | `false` | Verbose console output |

---

## Message Keys

All messages are configurable. Placeholders are replaced at runtime.

| Key | Placeholder | When Used |
|---|---|---|
| `reload` | | | Config reloaded |
| `pickup-cooldown` | `{time}` | Pickup attempted during cooldown |
| `pickup-success` | | | Spawner picked up successfully |
| `pickup-cancelled` | | | Player clicked NO in GUI |
| `pickup-inventory-full` | | | Items dropped due to full inventory |
| `admin-spawner-given` | `{type}` | Spawner given via `/cspawner` |
| `admin-no-permission` | | | Insufficient permission |
| `transfer-success-sender` | `{player}` | Transfer completed (sender) |
| `transfer-success-receiver` | `{sender}` | Transfer completed (receiver) |
| `transfer-no-permission` | | | Missing `orbspawn.transfer` |
| `transfer-hold-spawner` | | | Not holding a spawner |
| `transfer-not-owner` | | | Spawner belongs to someone else |
| `transfer-player-not-found` | `{player}` | Target player not online |
| `transfer-self` | | | Tried to transfer to self |

---

*Next: [How It Works | Pickup](how-it-works-pickup.md)*

# SpawnControl | Usage

## Commands

| Command | Permission | Description |
|---|---|---|
| `/spawncontrol version` | *(none)* | Shows plugin version and authors |
| `/spawncontrol reload` | `spawncontrol.admin` | Reloads `config.yml` and `spawns.yml` |
| `/spawncontrol spawn <entity> <amount>` | `spawncontrol.spawn` | Manually spawns entities at your location |
| `/spawncontrol zone create <name>` | `spawncontrol.admin` | Creates a new spawn zone |
| `/spawncontrol zone delete <name>` | `spawncontrol.admin` | Deletes an existing spawn zone |
| `/spawncontrol list` | `spawncontrol.admin` | Lists all active zones and their entity configs |

---

## Permissions

| Permission | Default | Description |
|---|---|---|
| `spawncontrol.admin` | OP | Full admin access | reload, zone management |
| `spawncontrol.spawn` | OP | Access to the manual spawn command |
| `spawncontrol.info` | `true` | View version info |

---

## Basic Workflow

1. Create a spawn zone with `/spawncontrol zone create <name>`
2. Define entity types, rates, and limits for that zone in `spawns.yml`
3. Reload with `/spawncontrol reload`
4. Optionally enable `log-spawns: true` in `config.yml` to monitor spawn activity in real time

---

*Next: [Configuration](configuration.md)*

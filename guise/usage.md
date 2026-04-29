# Guise | Usage

## Commands

| Command | Permission | Description |
|---|---|---|
| `/guise version` | *(none)* | Shows plugin version and authors |
| `/guise reload` | `guise.admin` | Reloads `config.yml` and `disguises.yml` |
| `/guise player <name>` | `guise.player` | Disguise as another player by username |
| `/guise mob <type>` | `guise.mob` | Disguise as a mob (e.g. `ZOMBIE`, `CREEPER`) |
| `/guise preset <name>` | `guise.preset` | Apply a preset disguise from `disguises.yml` |
| `/guise remove` | `guise.use` | Remove your current disguise |
| `/guise list` | `guise.admin` | List all currently active disguises on the server |
| `/guise check <player>` | `guise.admin` | Check what disguise a player is wearing |

---

## Permissions

| Permission | Default | Description |
|---|---|---|
| `guise.use` | `false` | Basic access | required to use `/guise remove` |
| `guise.player` | OP | Disguise as another player |
| `guise.mob` | OP | Disguise as a mob |
| `guise.preset` | OP | Apply preset disguises |
| `guise.admin` | OP | Full admin access |

---

## Basic Workflow

1. Run `/guise player Notch` to disguise as Notch | others will see you as that player
2. Run `/guise mob ZOMBIE` to disguise as a zombie
3. Run `/guise remove` to revert to your real appearance

---

*Next: [Configuration](configuration.md)*

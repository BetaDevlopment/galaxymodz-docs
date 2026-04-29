# EchoBlock | Configuration

## config.yml

```yaml
echoblock:
  debug: false
  default-cooldown: 5  # seconds | applies to all blocks unless overridden
```

---

## blocks.yml

Each entry maps an ID to a block location, trigger type, cooldown, and ordered action list:

```yaml
blocks:
  welcome_gate:
    world: world
    x: 100
    y: 64
    z: 200
    trigger: WALK_ON       # WALK_ON | INTERACT | BREAK
    cooldown: 10           # seconds (overrides default-cooldown)
    actions:
      - type: MESSAGE
        value: "&aWelcome to the arena, &e{player}&a!"
      - type: SOUND
        value: ENTITY_PLAYER_LEVELUP
      - type: COMMAND
        value: "give {player} golden_apple 1"
        delay: 20          # ticks (20 ticks = 1 second)

  danger_zone:
    world: world
    x: 300
    y: 70
    z: 300
    trigger: WALK_ON
    cooldown: 3
    actions:
      - type: MESSAGE
        value: "&cWarning: You are entering a danger zone!"
      - type: SOUND
        value: ENTITY_WITHER_AMBIENT
```

---

## Trigger Types

| Trigger | When it fires |
|---|---|
| `WALK_ON` | Player steps onto the block |
| `INTERACT` | Player right-clicks the block |
| `BREAK` | Player breaks the block |

---

## Action Types

| Type | Description | `value` format |
|---|---|---|
| `MESSAGE` | Sends a chat message to the triggering player | Any string | supports `&` colour codes and `{player}` |
| `BROADCAST` | Sends a message to all online players | Same as MESSAGE |
| `COMMAND` | Runs a console command | Command string | `{player}` is replaced with the player's name |
| `SOUND` | Plays a Bukkit sound to the player | Bukkit sound name (e.g. `ENTITY_PLAYER_LEVELUP`) |
| `DELAY` | Waits before executing the next action | Number of ticks |

---

*Next: [FAQ](faq.md)*

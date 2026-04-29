# SpawnControl | Configuration

## config.yml

```yaml
spawncontrol:
  debug: false
  log-spawns: false

  # Global spawn multiplier (0.5 = half rate, 2.0 = double rate)
  global-multiplier: 1.0

  # Enable region-based spawn zones
  zones-enabled: true

  # Entity types blocked from spawning entirely (server-wide)
  blacklist:
    - PHANTOM
    - GHAST
```

---

## spawns.yml

Define per-zone, per-entity spawn behaviour:

```yaml
zones:
  spawn_lobby:
    world: world
    min-x: -50
    max-x: 50
    min-z: -50
    max-z: 50
    entities:
      ZOMBIE:
        max-count: 10
        rate-multiplier: 0.5
      SKELETON:
        max-count: 5
        rate-multiplier: 1.0

  boss_arena:
    world: world
    min-x: 200
    max-x: 250
    min-z: 200
    max-z: 250
    entities:
      WITHER_SKELETON:
        max-count: 20
        rate-multiplier: 2.0
```

---

## Options Reference

### config.yml

| Key | Type | Default | Description |
|---|---|---|---|
| `debug` | boolean | `false` | Enable verbose debug logging |
| `log-spawns` | boolean | `false` | Log every spawn event to console |
| `global-multiplier` | float | `1.0` | Multiplier applied to all spawn rates globally |
| `zones-enabled` | boolean | `true` | Toggle zone-based spawn control on/off |
| `blacklist` | list | | | Entity types blocked from spawning server-wide |

### spawns.yml (per entity)

| Key | Type | Description |
|---|---|---|
| `max-count` | int | Maximum entities of this type allowed in the zone at once |
| `rate-multiplier` | float | Spawn rate multiplier for this entity within the zone |

---

*Next: [FAQ](faq.md)*

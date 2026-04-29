# BambEat — Configuration

## config.yml

```yaml
bambeat:
  # Hunger points restored (1 = half drumstick, 2 = 1 full drumstick)
  hunger: 3

  # Saturation restored
  saturation: 1.5

  # Cooldown between bamboo eating attempts (seconds, 0 = no cooldown)
  cooldown: 2

  # Only allow eating when the player is not full
  require-hunger: true

  # Potion effects applied on consumption (leave empty list for none)
  effects:
    - type: SPEED
      duration: 100   # ticks (20 ticks = 1 second)
      amplifier: 0    # 0 = level I, 1 = level II, etc.
    - type: REGENERATION
      duration: 40
      amplifier: 0
```

To disable all effects:

```yaml
effects: []
```

---

## Options Reference

| Key | Type | Default | Description |
|---|---|---|---|
| `hunger` | int | `3` | Hunger points restored per bamboo eaten |
| `saturation` | float | `1.5` | Saturation restored per bamboo eaten |
| `cooldown` | int | `2` | Seconds before the player can eat bamboo again |
| `require-hunger` | boolean | `true` | Prevent eating when hunger bar is full |
| `effects` | list | — | Potion effects applied on each bamboo eat |

---

*Next: [FAQ](faq.md)*

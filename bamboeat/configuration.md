# BambooEat | Configuration

## config.yml

```yaml
# Your license key — obtain via our Discord
license-key: "ENTER-YOUR-KEY-HERE"

eating:
  hunger-restore: 2          # Hunger points restored (2 = one full shank)
  saturation-restore: 0.4    # Saturation restored after eating
  cooldown-ticks: 10         # Cooldown between eats (10 ticks = 0.5 seconds)
  sound-volume: 1.0          # Eating sound volume (0.0 - 1.0)
  sound-pitch: 1.0           # Eating sound pitch (0.5 - 2.0)
  effect: NONE               # Potion effect on eat — NONE to disable
  effect-duration-ticks: 60  # Effect duration (20 ticks = 1 second)
  effect-amplifier: 0        # Effect level (0 = level I, 1 = level II)
```

---

## Options Reference

| Key | Type | Default | Description |
|---|---|---|---|
| `license-key` | string | — | Your BambooEat license key |
| `eating.hunger-restore` | int | `2` | Hunger points restored per bamboo eaten |
| `eating.saturation-restore` | float | `0.4` | Saturation restored per bamboo eaten |
| `eating.cooldown-ticks` | int | `10` | Ticks before the player can eat bamboo again |
| `eating.sound-volume` | float | `1.0` | Volume of the eating sound (0.0–1.0) |
| `eating.sound-pitch` | float | `1.0` | Pitch of the eating sound (0.5–2.0) |
| `eating.effect` | string | `NONE` | Potion effect applied on eat — use Bukkit effect name or `NONE` |
| `eating.effect-duration-ticks` | int | `60` | How long the effect lasts in ticks |
| `eating.effect-amplifier` | int | `0` | Effect strength (0 = level I) |

---

## Potion Effect Examples

```yaml
effect: SPEED
effect: REGENERATION
effect: POISON
effect: SLOWNESS
effect: JUMP_BOOST
```

Set `effect: NONE` to disable all effects.

---

## Applying Changes

Run `/bambooeat reload` in-game or console after saving `config.yml`. No restart needed.

---

*Next: [FAQ](faq.md)*

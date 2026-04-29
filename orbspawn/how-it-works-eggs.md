# OrbSpawn | How It Works: Egg Fuel System

Spawners are **active by default** | they spawn mobs at the standard Minecraft rate with no eggs required. Eggs are entirely optional and only exist to increase spawn speed, up to **10�| with 10 eggs**.

Right-clicking a placed spawner with the matching spawn egg adds fuel. Each egg reduces the spawn interval according to the formula:

```
delay = max(40, 400 / eggs) ticks     (20 ticks = 1 second)
```

---

## Speed Per Egg

| Eggs | Delay (ticks) | Interval | Multiplier |
|---|---|---|---|
| 0 | Default (Minecraft) | Varies* | | |
| 1 | 400 ticks | 20.0s | 1�| baseline |
| 2 | 200 ticks | 10.0s | 2�| |
| 3 | 133 ticks | ~6.7s | 3�| |
| 4 | 100 ticks | 5.0s | 4�| |
| 5 | 80 ticks | 4.0s | 5�| |
| 6 | 66 ticks | ~3.3s | 6�| |
| 7 | 57 ticks | ~2.9s | 7�| |
| 8 | 50 ticks | 2.5s | 8�| |
| 9 | 44 ticks | ~2.2s | 9�| |
| 10 | 40 ticks *(minimum)* | 2.0s | **10�| (maximum)** |

> \* Row 0: OrbSpawn does not set a custom delay when no eggs are present. The spawner uses Minecraft's default interval (varies by light level, mob cap, etc.). Adding the first egg sets a fixed 20-second interval, which may be slower or faster than the vanilla default depending on conditions.

---

## Egg Rules

- Only the **matching egg type** is accepted (e.g. a Cow egg only works on a Cow spawner)
- All eggs are consumed from your hand and stored as a **counter in the block PDC** (not inside the item)
- When a spawner is picked up, the egg count is **returned as physical egg items**
- The mob type is locked in PDC at creation | mismatched eggs are always rejected
- Eggs are **never** stored inside the spawner item | this is the core anti-duplication mechanism

---

*Next: [Ownership & Transfer](ownership.md)*

# BambooEat | Usage

## How to Eat Bamboo

Hold bamboo in your main hand and hold right-click. The bamboo will be consumed after the eat animation completes just like any vanilla food item.

- Works in your hand at all times regardless of hunger level
- Bamboo placed in non-hotbar slots is made edible automatically when picked up
- Switching away from bamboo mid-eat cancels the action
- Taking damage cancels the eat

---

## Third-Person Animation

If [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) is installed, nearby Java Edition players will see a proper eating arm animation when you consume bamboo. Bedrock players connected via Geyser see the animation through the [Geyser Extension](geyser.md) instead.

> ProtocolLib is a free, separate download. BambooEat works fully without it the animation is the only thing that requires it.

---

## Commands

| Command | Permission | Description |
|---|---|---|
| `/bambooeat reload` | `bambooeat.admin` | Reloads `config.yml`, re-validates license, re-checks for updates |

---

## Permissions

| Permission | Default | Description |
|---|---|---|
| `bambooeat.admin` | OP | Access to `/bambooeat reload` and in-game update notifications |

---

*Next: [Configuration](configuration.md)*

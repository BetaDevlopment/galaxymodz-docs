# BambooEat

> Bamboo. But make it food.

Vanilla Minecraft ignores bamboo as a food source entirely. BambooEat fixes that — players can hold bamboo and eat it like any other food item, complete with a satisfying crunch, custom particles, and fully configurable hunger and effect values.

Simple to install, zero friction for players, and entirely configurable by you.

---

## What does it add?

Out of the box, BambooEat turns bamboo into a proper food item. Right-click to eat, hear the crunch, see the particles, get the hunger back. Everything about how it behaves — hunger restored, saturation, cooldown, potion effects — is yours to configure.

**Highlights:**

**Sounds & visuals that feel right**
Custom crunchy eating sounds and block-break particles play on consumption. It doesn't feel bolted-on — it feels like it belongs.

**Third-person eating animation** *(optional — requires ProtocolLib)*
Other players nearby see a proper eating arm animation when someone consumes bamboo, matching vanilla food behaviour. Powered by [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) as a soft dependency — the plugin works fully without it installed.

**Automatic update checker**
BambooEat checks for new versions on startup and on `/bambooeat reload`. Admins receive an in-game notification when a newer version is available.

**Fully configurable values**
Set exactly how much hunger and saturation bamboo restores. Stack on potion effects like Speed or Regeneration, or leave it clean. It's all in `config.yml`.

**Optional cooldown**
Prevent spam-eating with a configurable cooldown between bites.

**Bedrock support (Geyser Extension)**
Running Geyser? The optional Geyser Extension brings the full eating hand animation to Bedrock players — identical to Java Edition. Available as a +$1.99 add-on at checkout. [Learn more](geyser.md)

---

## Perfect for

- Survival servers that want an early-game food source in jungle biomes
- Bamboo-themed custom gamemodes or progression systems
- Any server looking for a small, polished quality-of-life addition

---

## Changelog

### v1.6.5 | Animation, Update Checker & Bug Fixes
*Released 2 May 2026*

- Third-person eating animation via [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) (optional soft dependency)
- Automatic update checker with in-game admin notifications
- Fixed: startup window where bamboo was edible before license validation
- Fixed: bamboo picked up off the ground sometimes not becoming edible
- Fixed: eating cooldown bypass in rare timing cases
- Fixed: HTTP connection leak in license checker

> ⚠ ProtocolLib animation support is experimental in this release. The plugin works fully without ProtocolLib installed.

### v1.1.0 | Geyser Extension & Full Bedrock Support
*Released 27 April 2026*

- Geyser Extension released — Bedrock players now get the full eating hand animation
- Bundled resource pack served automatically to connecting Bedrock clients
- Available as a paid add-on (+$1.99) at checkout
- Zero performance impact — one custom item and one resource pack registered on startup

### v1.0.0 | Initial Release

- Bamboo as a fully functional food item
- Custom crunchy eating sounds
- Block-break particles while eating
- Configurable hunger and saturation restore
- Optional potion effects on eat
- Paper 1.21.0–1.21.11 support

---

## Get BambooEat

Available on BuiltByBit:
[builtbybit.com/resources/bambooeat-edible-bamboo-plugin.101395](https://builtbybit.com/resources/bambooeat-edible-bamboo-plugin.101395/)

---

## Requirements

- Java 17+
- Paper 1.21.0–1.21.11
- [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) *(optional — third-person animation only)*
- Geyser *(optional — required for the [Geyser Extension](geyser.md))*

---

## Developers

Built by **GalaxyModz** & **Frostbyte**
Questions? Join us at **discord.gg/galaxymodz**

---

*Next: [Installation](installation.md)*

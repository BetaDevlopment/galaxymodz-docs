# EchoBlock — Overview

**EchoBlock** is a GalaxyModz plugin that turns any block in your world into a trigger. When players walk on, interact with, or break an Echo Block, it fires a configurable chain of actions — messages, sounds, commands, and more.

---

## What It Does

EchoBlock links physical blocks to event chains defined in `blocks.yml`. Each block has a trigger type and an ordered list of actions with optional delays and per-block cooldowns.

**Key Features:**

- Register any block as an Echo Block using a single command
- Chain multiple actions per trigger (messages, sounds, commands, broadcasts)
- Per-block cooldown and action delay support
- Persistent — blocks survive server restarts
- Hot-reload support — no restart needed after config changes

---

## Use Cases

- Interactive adventure map triggers
- Announcement zones (entering a region plays a sound and sends a message)
- Automate command execution on block interaction

---

## Requirements

- Java 17+
- Paper / Spigot 1.20+

---

## Developers

Built by **GalaxyModz** & **Frostbyte**

---

*Next: [Installation](installation.md)*

# BambEat — Geyser Extension

**v1.1.0** adds a Geyser Extension that gives Bedrock players the full bamboo eating experience, matching Java Edition exactly.

---

## What It Does

Without the extension, Bedrock players can eat bamboo (the mechanic works) but do not see the hand animation because Bedrock requires a custom item definition for the animation to play. The Geyser Extension solves this.

**What it adds:**
- Full eating hand animation for Bedrock players — identical to Java Edition
- Bundled resource pack served automatically to connecting Bedrock clients — no manual installation needed by players
- Zero performance impact — registers one custom item and one resource pack on startup, nothing else

---

## How to Get It

The Geyser Extension is available as a **paid add-on** for **+$1.99** at checkout.

> If you run a Java-only server you are not paying for something you will never use. If you do run Geyser, the +$1.99 gets you the full experience for all your players.

---

## Installation

1. Purchase the Geyser Extension add-on
2. Place the extension JAR in the same `/plugins` folder as Geyser (see [proxy/network setup](#proxy-and-network-setup) below if you use one)
3. Restart the server — the extension registers automatically
4. Bedrock clients connecting will receive the resource pack automatically

No additional configuration is required.

---

## Requirements

- BambEat v1.1.0 or newer
- Geyser installed and running (standalone, Velocity, BungeeCord, or any proxy)

---

## Proxy and Network Setup

If you run a proxy network (Velocity, BungeeCord, or any multi-server setup where Geyser sits at the proxy level), the extension still works — you just need to place the files in the right locations.

### How it works on a proxy

When Geyser runs as a proxy plugin:
- Bedrock players connect to Geyser at the proxy level
- Geyser translates packets between Bedrock and whichever backend Java server the player is on
- The Geyser Extension registers a custom item mapping at proxy startup — it tells Geyser: *"any bamboo stack that has a `minecraft:food` component → show Bedrock clients a custom food item"*

This registration happens once when Geyser initialises (`GeyserDefineCustomItemsEvent`). It does not matter which backend server the player is connected to at the time. Once registered, the custom item mapping applies globally — all Bedrock players on any backend server will see the animation correctly.

### Where each file goes

| File | Where it goes |
|---|---|
| `BambooEat-GeyserExtension.jar` | Proxy server `/plugins` folder, alongside Geyser |
| `BambooEat.jar` (the main plugin) | Each backend server where you want bamboo to be edible |

### One thing to keep in mind

The extension maps bamboo to a food item by detecting the `minecraft:food` data component on the item stack. BambEat (on the backend server) is what attaches that component — Geyser at the proxy level sees it when forwarding item packets to the Bedrock client.

This means:
- On backend servers **with** BambEat installed: bamboo is edible and Bedrock players see the full animation
- On backend servers **without** BambEat installed: bamboo is not edible and no animation plays — which is the expected behaviour

---

*Back to [Overview](overview.md)*

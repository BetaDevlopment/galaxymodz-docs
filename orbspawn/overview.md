# OrbSpawn | Overview

**OrbSpawn** is a premium GalaxyModz plugin that delivers fully exploit-proof spawner management for Minecraft servers. It gives administrators complete control over who can place, pick up, fuel, and transfer mob spawners | with no duplication exploits, no ownership bypasses, and no natural-spawner abuse.

> **CraftPort Early Access** | OrbSpawn is currently available exclusively to CraftPort members before its public release. CraftPort does not sell the plugin; it is a partner server with early access rights.

---

## Plugin Info

| Property | Value |
|---|---|
| Plugin Version | v3.5 |
| Minecraft API | 1.21.4 (Spigot / Paper) |
| Java Version | 17+ |
| Author | GalaxyModz Development |
| Early Access | Yes | available before public release |
| Support | discord.gg/galaxymodz |
| License | Commercial | License Key Required |

---

## Features Overview

### Natural Spawner Blocking
All naturally generated spawners (dungeons, mineshafts, bastions) are permanently locked. They cannot be broken, picked up, or fuelled.

### Spawner Pickup System
Authorised players pick up their own spawner via **Shift + Right-Click** (empty hand) or **Shift + Left-Click** (pickaxe). A GUI confirmation prevents accidental pickups.

### Egg Fuel System
Spawners are active by default and will spawn mobs at the standard Minecraft rate without any eggs. Eggs are entirely optional | each egg added increases spawn speed, up to **10�| with 10 eggs**. All eggs are fully returned on pickup.

### UUID Ownership System
Every spawner is cryptographically tied to its owner's UUID. Name changes and Bedrock cross-play do not break ownership | UUID never changes.

### Spawner Transfer
Owners can transfer a spawner they are holding to any online player. Admins can transfer any spawner regardless of ownership.

### Admin Give Command
`/cspawner` gives any player a spawner for any of the **78 supported mob types**, with optional extra eggs.

### Bedrock / Geyser Support
Full support for Geyser players. The dot-prefix is stripped in all displays and both forms are tried on lookups. Ownership is UUID-based so prefix removal is irrelevant.

### Anti-Duplication Protections
- Pistons cannot move spawners
- Explosions cannot drop spawner items
- Egg fuel is never stored in the spawner item
- All known duplication exploits are blocked

### Pickup Cooldown
Configurable cooldown (default 3 seconds) prevents pickup spam.

### Tebex Integration
Native support for TebexCheckout and BuycraftX.

### Stacker Compatibility
Compatible with RoseStacker and WildStacker.

### Thread Safety
All operations are thread-safe (ConcurrentHashMap). Tested with 30+ concurrent players.

---

> **Important | Egg Behaviour**
> Spawners no longer come with eggs bundled when given via `/cspawner`. This change was made to close a major duplication exploit. Spawners are active by default. Eggs only exist to increase spawn speed. Use `/cspawner <player> <mob> extraegg <n>` if you want to give eggs alongside a spawner.

---

*Next: [Installation](installation.md)*

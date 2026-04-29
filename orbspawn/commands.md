# OrbSpawn — Commands

## /orbspawn reload

Reloads `config.yml`. All cached values refresh immediately — no server restart needed.

| | |
|---|---|
| Permission | `orbspawn.reload` |
| Default | OP |
| Aliases | `/obs reload`, `/ospawn reload` |

```
/orbspawn reload
/obs reload
```

---

## /orbspawn transfer \<player\>

Transfers ownership of the spawner in your main hand to the specified player. You must own the spawner, or have `orbspawn.admin` to bypass the ownership check.

| | |
|---|---|
| Permission | `orbspawn.transfer` |
| Default | All players |
| Aliases | `/obs transfer`, `/ospawn transfer` |

```
/orbspawn transfer Steve
/obs transfer BedrockPlayer
```

> Bedrock players can be addressed by their clean name (without dot prefix). Both forms are resolved automatically.

---

## /cspawner (no arguments)

Opens an interactive mob selection menu listing all 78 supported spawner types and all online players.

| | |
|---|---|
| Permission | `orbspawn.admin` |
| Default | OP |
| Aliases | `/customspawner`, `/adminspawner` |
| Note | Players only — not usable from console |

---

## /cspawner \<mob\>

Gives **yourself** a spawner of the specified mob type. No eggs are included — the spawner runs at default Minecraft rate.

| | |
|---|---|
| Permission | `orbspawn.admin` |
| Default | OP |

```
/cspawner warden
/cspawner zombie
```

---

## /cspawner \<player\> \<mob\>

Gives the target player a spawner. No eggs included. Spawner is assigned to the target's UUID. Works from console.

| | |
|---|---|
| Permission | `orbspawn.admin` |
| Default | OP |

```
/cspawner Steve cow
/cspawner BedrockPlayer zombie
```

---

## /cspawner \<player\> \<mob\> extraegg \<n\>

Gives the target player a spawner plus `n` extra spawn eggs. Use this when you specifically want to pre-supply eggs.

| | |
|---|---|
| Permission | `orbspawn.admin` |
| Default | OP |

```
/cspawner Steve zombie extraegg 3
/cspawner Notch warden extraegg 9
```

> `n` must be a positive integer. Eggs are given as separate inventory items — not stored in the spawner item itself. The player must right-click the placed spawner with the eggs to fuel it.

---

## /fixspawners

Scans your inventory and marks any untagged spawner items as OrbSpawn-allowed. Use this when importing spawners from other plugins or legacy worlds.

| | |
|---|---|
| Permission | `orbspawn.admin` |
| Default | OP |

```
/fixspawners
```

---

*Next: [Permissions](permissions.md)*

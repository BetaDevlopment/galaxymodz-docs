# EchoBlock

> Turn any block into a trigger. Walk on it, click it, break it | and watch your server come alive.

EchoBlock lets you attach event chains to any block in your world. No scripting, no complex setup | just place a block, register it with one command, and define what happens in a simple config file.

---

## What can you build with it?

The short answer: anything that reacts to a player.

- A pressure plate at the dungeon entrance that plays an ominous sound and flashes a warning message
- A hidden trigger block that runs a console command when a player steps on it
- An info board that broadcasts a message to the whole server when someone interacts with it
- Event zones that fire timed action sequences | sounds, messages, and commands with delays between them

If it involves a block and a player, EchoBlock can handle it.

---

## Features

**Block registration**
Register any block in the world as an Echo Block with a single command | no coordinates to type, just look at the block and run `/echoblock set <id>`.

**Action chains**
Each Echo Block runs an ordered list of actions when triggered. Mix and match messages, sounds, commands, broadcasts, and delays in any order you want.

**Three trigger types**
Choose how each block fires | when a player walks on it (`WALK_ON`), right-clicks it (`INTERACT`), or breaks it (`BREAK`).

**Per-block cooldowns**
Set a cooldown per block so actions don't fire every tick. A global default is set in `config.yml` and can be overridden per block.

**Persistent & hot-reloadable**
Echo Blocks survive server restarts. Config changes apply instantly with `/echoblock reload` | no downtime.

---

## Get EchoBlock

Available on BuiltByBit:
[builtbybit.com/resources/echoblock-capture-your-last-words.101654](https://builtbybit.com/resources/echoblock-capture-your-last-words.101654/)

---

## Requirements

- Java 17+
- Paper / Spigot 1.20+

---

## Developers

Built by **GalaxyModz** & **Frostbyte**
Questions? Join us at **discord.gg/galaxymodz**

---

*Next: [Installation](installation.md)*

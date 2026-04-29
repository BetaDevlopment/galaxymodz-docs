# Guise | Configuration

## config.yml

```yaml
guise:
  debug: false

  # Whether the disguised player can see their own disguise (first-person)
  self-view: false

  # Automatically remove disguise when the player dies
  remove-on-death: true

  # Automatically remove disguise when the player changes world
  remove-on-world-change: false

  # Prevent mobs from targeting disguised players
  mob-ignore-disguise: false
```

---

## disguises.yml

Define named preset disguises that players can apply with `/guise preset <name>`:

```yaml
presets:
  ghost:
    type: MOB
    entity: PHANTOM
    name: "&7Ghost"

  admin_incognito:
    type: PLAYER
    skin: "Notch"
    name: "&8Unknown"

  panda_suit:
    type: MOB
    entity: PANDA
    name: "&fPanda"
```

Apply a preset with:

```
/guise preset ghost
```

---

## Options Reference

### config.yml

| Key | Type | Default | Description |
|---|---|---|---|
| `debug` | boolean | `false` | Enable verbose debug logging |
| `self-view` | boolean | `false` | Allow the wearer to see their own disguise |
| `remove-on-death` | boolean | `true` | Strip disguise when the player dies |
| `remove-on-world-change` | boolean | `false` | Strip disguise when the player changes world |
| `mob-ignore-disguise` | boolean | `false` | Mobs will not target disguised players |

### disguises.yml (per preset)

| Key | Description |
|---|---|
| `type` | `MOB` or `PLAYER` |
| `entity` | Bukkit entity type (for `MOB` type) |
| `skin` | Minecraft username to pull skin from (for `PLAYER` type) |
| `name` | Display name shown above the disguise | supports `&` colour codes |

---

*Next: [FAQ](faq.md)*

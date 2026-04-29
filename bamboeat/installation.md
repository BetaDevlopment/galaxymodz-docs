# BambEat | Installation

## Requirements

- Java 17+
- Paper / Spigot 1.20+

---

## Steps

### 1. Download

Get the latest `BambEat.jar` from the GalaxyModz releases page.

### 2. Add to Plugins Folder

Drop the jar into your server's `/plugins` directory.

### 3. Restart the Server

Restart your server. BambEat will generate its config automatically:

```
/plugins/BambEat/
└── config.yml
```

### 4. Verify Installation

Run in-game or in the server console:

```
/bambeat version
```

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Plugin not loading | Confirm Paper/Spigot 1.20+ with Java 17+ |
| Bamboo not edible | Check that the player has the `bambeat.eat` permission |
| Config not generated | Delete `/plugins/BambEat/` and restart |

---

*Next: [Usage](usage.md)*

# EchoBlock — Installation

## Requirements

- Java 17+
- Paper / Spigot 1.20+

---

## Steps

### 1. Download

Get the latest `EchoBlock.jar` from the GalaxyModz releases page.

### 2. Add to Plugins Folder

Drop the jar into your server's `/plugins` directory.

### 3. Restart the Server

Restart your server. EchoBlock will generate its configuration files automatically:

```
/plugins/EchoBlock/
├── config.yml
└── blocks.yml
```

### 4. Verify Installation

Run in-game or in the server console:

```
/echoblock version
```

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Plugin not loading | Confirm Paper/Spigot 1.20+ with Java 17+ |
| Config not generated | Delete `/plugins/EchoBlock/` and restart |
| Blocks not triggering | Check `blocks.yml` coordinates and trigger type are correct |

---

*Next: [Usage](usage.md)*

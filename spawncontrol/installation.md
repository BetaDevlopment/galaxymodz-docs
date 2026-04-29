# SpawnControl | Installation

## Requirements

- Java 17+
- Paper / Spigot 1.20+
- Server restart access

---

## Steps

### 1. Download

Get the latest `SpawnControl.jar` from the official GalaxyModz releases page.

### 2. Add to Plugins Folder

Drop the jar into your server's `/plugins` directory:

```
server/
└── plugins/
    └── SpawnControl.jar
```

### 3. Restart the Server

Restart your server. SpawnControl will generate its default configuration files on first run:

```
/plugins/SpawnControl/
├── config.yml
└── spawns.yml
```

### 4. Verify Installation

Run in-game or in the server console:

```
/spawncontrol version
```

You should see the plugin version and authors printed to confirm it loaded correctly.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Plugin not loading | Confirm your server is running Paper/Spigot 1.20+ with Java 17+ |
| Config not generated | Delete `/plugins/SpawnControl/` and restart to regenerate defaults |
| Command not found | Check console for startup errors | the plugin may have failed to enable |

---

*Next: [Usage](usage.md)*

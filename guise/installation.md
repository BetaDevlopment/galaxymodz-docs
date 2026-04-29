# Guise | Installation

## Requirements

- Java 17+
- Paper / Spigot 1.20+
- ProtocolLib (required | must be installed first)

---

## Steps

### 1. Install ProtocolLib

Download and install [ProtocolLib](https://www.spigotmc.org/resources/protocollib.1997/) into your `/plugins` folder if you haven't already.

### 2. Download Guise

Get the latest `Guise.jar` from the GalaxyModz releases page.

### 3. Add to Plugins Folder

Drop `Guise.jar` into your server's `/plugins` directory.

### 4. Restart the Server

Restart your server. Guise will generate its configuration files:

```
/plugins/Guise/
├── config.yml
└── disguises.yml
```

### 5. Verify Installation

Run in-game or in the server console:

```
/guise version
```

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Plugin not loading | Confirm ProtocolLib is installed and up to date |
| Disguises not applying visually | Confirm ProtocolLib version is compatible with your server version |
| Config not generated | Delete `/plugins/Guise/` and restart |

---

*Next: [Usage](usage.md)*

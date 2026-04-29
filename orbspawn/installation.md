# OrbSpawn | Installation

## Requirements

| Component | Requirement |
|---|---|
| Minecraft Server | Spigot or Paper 1.21.4 or newer |
| Java | 17+ (Java 21 recommended) |
| OrbSpawn JAR | `OrbSpawn-3.5.jar` (obfuscated release) |
| License Key | Valid key provided by GalaxyModz Development |

---

## Installation Steps

### 1. Add the JAR

Place `OrbSpawn-3.5.jar` in your server's `/plugins/` folder.

### 2. First Start

Start the server once. OrbSpawn generates its configuration file:

```
/plugins/OrbSpawn/
└── config.yml
```

### 3. Enter Your License Key

Open `config.yml` and enter your license key:

```yaml
license-key: "YOUR-LICENSE-KEY-HERE"
```

### 4. Restart or Reload

Save and restart the server, or run:

```
/orbspawn reload
```

### 5. Verify

Confirm the console shows:

```
Licence validated successfully
```

---

> **Warning**
> The plugin will not start without a valid license key. Ensure your server has outbound internet access for license validation.

---

*Next: [Commands](commands.md)*

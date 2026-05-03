# BambooEat | Installation

## Requirements

| Requirement | Version | Notes |
|---|---|---|
| Java | 17+ | Required |
| Paper | 1.21.0–1.21.11 | Required |
| [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) | Latest | Optional enables third-person eating animation |
| Geyser | Any | Optional required for the [Geyser Extension](geyser.md) |

---

## Steps

### 1. Download

Get the latest `BambooEat-1.6.5.jar` from the BuiltByBit resource page.

### 2. Add to Plugins Folder

Drop the jar into your server's `/plugins` directory.

```
/plugins/
└── BambooEat-1.6.5.jar
└── ProtocolLib.jar   ← optional, for third-person animation
```

### 3. Restart the Server

Restart your server. BambooEat will generate its config automatically:

```
/plugins/BambooEat/
└── config.yml
```

### 4. Enter Your License Key

Open `plugins/BambooEat/config.yml` and replace the placeholder with your license key:

```yaml
license-key: "YOUR-KEY-HERE"
```

Then **restart the server again** to apply the license key.

> **Note:** `/bambooeat reload` does not apply license key changes. You must do a full server restart, or you will get an error.

### 5. Verify Installation

You should see the following lines in your console on startup:

```
[BambooEat] ==========================================
[BambooEat]  BambooEat v1.6.5 - GalaxyModz Development
[BambooEat] ==========================================
[BambooEat] License validated. Plugin active.
[BambooEat] Plugin is up to date (v1.6.5).
```

If ProtocolLib is installed you will also see:

```
[BambooEat] ProtocolLib found third-person eating animation enabled.
```

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Plugin not loading | Confirm Paper 1.21+ with Java 17+ |
| License invalid | Check your key in `config.yml` join Discord for a new key |
| Bamboo not edible | Ensure the license is validated (check console on startup) |
| No eating animation | Install [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) it is a separate download |
| Config not generated | Delete `/plugins/BambooEat/` and restart |

---

*Next: [Usage](usage.md)*

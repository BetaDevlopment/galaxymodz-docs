# EchoBlock | Usage

## Commands

| Command | Permission | Description |
|---|---|---|
| `/echoblock version` | *(none)* | Shows plugin version and authors |
| `/echoblock reload` | `echoblock.admin` | Reloads `config.yml` and `blocks.yml` |
| `/echoblock set <id>` | `echoblock.admin` | Registers the block you are looking at as an Echo Block |
| `/echoblock remove <id>` | `echoblock.admin` | Removes an Echo Block by ID |
| `/echoblock list` | `echoblock.admin` | Lists all registered Echo Blocks and their trigger types |
| `/echoblock info <id>` | `echoblock.admin` | Shows full details and action list for a block |

---

## Permissions

| Permission | Default | Description |
|---|---|---|
| `echoblock.admin` | OP | Full admin access |
| `echoblock.info` | `true` | View version info |

---

## Basic Workflow

1. Stand in front of a block and run `/echoblock set myblock`
2. Open `blocks.yml` and define the trigger type and action list for `myblock`
3. Reload with `/echoblock reload`
4. Interact with the block to fire the action chain

---

*Next: [Configuration](configuration.md)*

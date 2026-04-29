# OrbSpawn — Bedrock / Geyser Support

OrbSpawn has full support for Geyser (Bedrock) players. Ownership is UUID-based, so the Geyser dot-prefix is irrelevant to how spawners are tracked.

---

## Behaviour by Area

| Area | Behaviour |
|---|---|
| Player Lookup | Both `Steve` and `.Steve` are tried automatically on transfer and `/cspawner` |
| Display Names | All messages, GUI text, and item lore always show clean names (dot-prefix stripped) |
| Ownership | UUID-based — unaffected by dot-prefix or its removal |
| Tab Completion | Bedrock player `.Steve` appears as `Steve` |
| No-prefix servers | Servers that remove the Geyser dot prefix are fully supported |

---

> **Note**
> If a server removes the Geyser dot prefix and a Bedrock and Java player share the same username, Minecraft itself prevents them from being online simultaneously. This is a server configuration concern, not an OrbSpawn issue.

---

*Next: [Security & Anti-Exploit](security.md)*

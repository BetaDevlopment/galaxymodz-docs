# BambooEat | FAQ

**Q: Do I need ProtocolLib?**
A: No. ProtocolLib is completely optional. Without it, bamboo is fully edible and everything works normally only the third-person eating animation (visible to other nearby Java players) requires it. [Download ProtocolLib](https://github.com/dmulloy2/ProtocolLib)

---

**Q: The eating animation is not showing for other players. What's wrong?**
A: Make sure [ProtocolLib](https://github.com/dmulloy2/ProtocolLib) is installed on your server. On startup you should see:
```
[BambooEat] ProtocolLib found third-person eating animation enabled.
```
If you see `ProtocolLib not found`, ProtocolLib is missing or failed to load.

---

**Q: Is the ProtocolLib animation stable?**
A: It works correctly in most setups but is still considered experimental in v1.6.5. If you experience any issues, removing ProtocolLib will not affect any other functionality.

---

**Q: Does BambooEat work with Bedrock players (Geyser)?**
A: Yes. Java players use ProtocolLib for the animation. Bedrock players get their animation through the [Geyser Extension](geyser.md) add-on instead. The two systems are independent and do not interfere with each other.

---

**Q: Does BambooEat work with custom food plugins?**
A: It may conflict with plugins that override item use events. Test on a staging server first.

---

**Q: Can I disable the eating sound?**
A: Set `sound-volume: 0.0` in `config.yml` to effectively mute the eating sound.

---

**Q: Can pandas also benefit from the config values?**
A: BambooEat targets player consumption only. Vanilla panda behaviour is unaffected.

---

**Q: How do I remove all potion effects?**
A: Set `effect: NONE` in `config.yml`:
```yaml
effect: NONE
```

---

**Q: How do I reload the config without restarting?**
A: Run `/bambooeat reload` in-game or console. This reloads `config.yml`, re-validates your license, and re-checks for updates.

---

**Q: How do I report a bug?**
A: Join the Discord and open a support ticket, or contact **GalaxyModz** directly.

---

*Back to [Overview](overview.md)*

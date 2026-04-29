# SpawnControl — FAQ

**Q: Does SpawnControl work with other spawn-related plugins?**
A: It may conflict with plugins that directly modify spawn rates (e.g., MobControl, ClearLagg). Test compatibility on a staging server first.

---

**Q: Can I use SpawnControl on multiple worlds?**
A: Yes. Zones are world-specific — just specify the `world` key in `spawns.yml` for each zone.

---

**Q: Will SpawnControl affect natural mob caps?**
A: SpawnControl works alongside Minecraft's native mob caps. The `max-count` setting adds an additional layer of control on top of vanilla limits.

---

**Q: How do I disable SpawnControl for a specific world?**
A: Simply don't define any zones for that world in `spawns.yml`. SpawnControl only affects zones explicitly configured.

---

**Q: The plugin isn't reducing spawns — what's wrong?**
A: Ensure `zones-enabled: true` in `config.yml`, and that your coordinates in `spawns.yml` correctly cover the area. Use `/spawncontrol list` to verify zones are loaded.

---

**Q: How do I report a bug?**
A: Contact **GalaxyModz** or **Frostbyte** directly through your support channel or issue tracker.

---

*Back to [Overview](overview.md)*

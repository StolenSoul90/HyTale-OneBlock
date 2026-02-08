# v.0.1.0 - Foundation (you are here)
- Clean workspace, build compiles, server runs
- Empty plugin class, manifest, asset folders
- First commit baseline
# v0.2.0 - Plugin Lifecycle
- OneBlock.java loads and unloads properly
- Server logs confirm your plugin is active
- Basic command registration (even just `/oneblock` that responds with "Hello")
# v0.3.0 - World Isolation
- Player joins and gets teleported to a void/empty world
- Single block placed at spawn (the "one block")
- Each player gets their own island instance or assigned location
# v0.4.0 - Block Breaking Core Loop
- Breaking the one block causes it to respawn
- Block type changes based on a phase/progression table
- Track how many blocks each player has broken
# v0.5.0 - Phase System
- Define phases (Grass -> Wood -> Stone -> Ore -> Nether-equivalent, etc)
- Each phase has a weighted loot table of block types
- Players progress through phases based on blocks broken
# v0.6.0 - Item Drops
- Breaking blocks can drop items (tools, food, seeds, materials)
- Drop tables per phase with rarity weights
- inventory management works correctly
# v0.7.0 - Mob Spawning
- Breaking blocks has a chance to spawn mobs
- Mob types tied to current phase
- Hostile and passive mobs balanced per phase
# v0.8.0 - Persistence
- Player progress saves and loads between sessions
- Island state persists across server restarts
- Config file for customizing phases, drops, and rates
# v0.9.0 - Custom Assets
- Custom block textures or models if needed
- UI elements, sounds, or particles for block regeneration
- This is where your Common/ and Server/ folders get populated
# v1.0.0 - Release
- All phases complete and balanced
- Edge cases handled (death, disconnect mid-break, etc.)
- README updated with install instructions for other players
- First tagged release on GitHub -> `git tag v1.0.0`
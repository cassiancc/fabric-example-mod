# Fabric Example Mod

## Setup

For setup instructions please see the [fabric documentation page](https://docs.fabricmc.net/develop/getting-started/setting-up) that relates to the IDE that you are using.

## Migration

If you're feeling experimental, Fabric is currently testing a no-remap version of Loom that can be used on the experimental releases. For most, the process should be as simple.

- Change the version of Loom you are using to `id "net.fabricmc.fabric-loom" version "1.14-SNAPSHOT"`
- Update Fabric Loader to 0.18.1 or above
- Remove the `mappings` line from your `build.gradle`
- Replace any instances of `modImplementation` or `modCompileOnly` with `implementation` and `compileOnly`
- Replace any mods using intermediary mappings (most Fabric mods) with unobfuscated builds, i.e. [Fabric API](https://github.com/FabricMC/fabric/releases/tag/0.139.4%2B1.21.11_unobfuscated).
- Replace any mentions of `remapJar` with `jar`

## License

This template is available under the CC0 license. Feel free to learn from it and incorporate it in your own projects.

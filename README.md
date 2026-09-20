# Offhand Shift-Click (Fabric, Minecraft 26.1.2)

Shift-click an item in your own inventory screen to put it in your off hand.
Chests, furnaces and other containers behave like vanilla.
Open Mod Menu -> Offhand Shift-Click -> configure.

## Config
- Enabled: master switch
- List mode: "Everything except deny list" (default) or "Only allow list"
- Entries (one per line): `minecraft:diamond`, `#minecraft:swords` (tag), `create:*` (whole mod)

## Play requirements
Java 25, Fabric Loader 0.19.3+, Fabric API, Cloth Config API, Mod Menu (all for 26.1.x).

## Build
Push to GitHub with the .github/workflows/build.yml workflow, then download the artifact from the Actions tab.
26.1+ is unobfuscated: fabric-loom plugin, Mojang names. In 26.1.x slot clicks still use ClickType /
handleInventoryMouseClick (renamed ContainerInput / handleContainerInput in 26.2).

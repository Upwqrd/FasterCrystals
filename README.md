[![Modrinth](https://img.shields.io/modrinth/v/FasterCrystals?label=Modrinth&style=for-the-badge)](https://modrinth.com/plugin/fastercrystals)

# FasterCrystals
This fork passes placements to LegacyGrim's existing limiter through `EntityPlaceEvent`.
Set `CrystalPlaceLimit` in `plugins/GrimAC/config.yml` and use `/grim reload`; native placements and both FasterCrystals hands share one budget. `0` disables the limit.
Requires [LegacyGrim](https://github.com/Upwqrd/LegacyGrim) and PacketEvents. No agents or reflection.

This plugin allows high ping players to crystal quickly by processing the left/right clicks *as the packets come in*.
This means that the server does not have to rely on the client's attack packet to destroy a crystal, and also does not have to rely on the client's block interact packet to place a crystal.
This is the main reason why high ping players cannot crystal quickly normally; the crystals take too long to get destroyed/placed on their clients.

The plugin will only function on Paper (or its compatible forks) and Folia servers.

## Installation
[PacketEvents](https://github.com/retrooper/packetevents/releases) **must** be installed for this plugin to work.

## Building
Clone the repository, `cd` into it, then `./gradlew build`.

The output file will be located in `./build/libs/FasterCrystals-VERSION.jar`.

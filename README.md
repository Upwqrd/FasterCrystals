# FasterCrystals для LegacyGrim

Форк [FasterCrystals 2.2.1](https://github.com/mcpvp-club/FasterCrystals/tree/v2.2.1).

Использует общий `CrystalPlaceLimit` из `plugins/GrimAC/config.yml`: обычные установки и FasterCrystals, обе руки вместе. `0` отключает лимит; `/grim reload` применяет изменение.

Требуются [LegacyGrim](https://github.com/Upwqrd/LegacyGrim) и [PacketEvents](https://github.com/retrooper/packetevents/releases). Замените обычный FasterCrystals этим форком.

Сборка: Java 21, `./gradlew build`. JAR: `build/libs/FasterCrystals-2.2.1-legacygrim1.jar`.

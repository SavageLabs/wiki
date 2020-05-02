---
title: SkyblockX
description: 
published: 1
date: 2020-05-02T01:05:36.069Z
tags: 
---

<h3>Last Updated: v1.4.2-alpha</h3>
<h2>config.json</h2>

```json
{
  "defaultWorld": "world",
  "islandMaxSizeInBlocks": 100,
  "islandPaddingSizeInBlocks": 20,
  "openIslandMenuOnBaseCommand": true,
  "skyblockWorldName": "skyblockx",
  "skyblockWorldNameNether": "skyblockx_nether",
  "preventFallingDeaths": true,
  "useFallingDeathCommands": false,
  "fallingDeathPreventionCommands": [
    "eco take {player} 100"
  ],
  "skyblockDeathTeleport": true,
  "levelIncrementFactor": 25,
  "islandResetCoolDownSeconds": 21600,
  "islandDeleteClearInventory": true,
  "islandDeleteClearEnderChest": true,
  "chestRows": {
    "1": 3,
    "2": 4,
    "3": 5,
    "4": 5,
    "5": 6
  },
  "defaultMaxCoopPlayers": 3,
  "defaultMaxIslandHomes": 3,
  "helpGeneratorPageEntries": 10,
  "defaultIslandMemberLimit": 3,
  "islandOreGeneratorEnabled": true,
  "skyblockWorldBiome": "PLAINS",
  "islandTopIslandCalculationSpeedIntervalMilis": 10000,
  "islandTopLineFormat": "&b{rank}&7. &7{leader}'s island &b(${amount})&7.",
  "useIslandTopHeadMessage": true,
  "islandTopHeadMessage": "&b&lTop Islands &7&o((By block Value))",
  "useIslandTopHeaderBar": true,
  "barLength": 50,
  "islandTopbarElement": "&8&m=",
  "islandTopTooltip": [
    "&7Leader: &b{leader}",
    "&7Dirt: &b{DIRT}",
    "&7Creeper Spawner: &b{CREEPER}",
    "&7Zombie Spawner: &b{ZOMBIE}",
    "&7Skeleton Spawner: &b{SKELETON}",
    "&7Diamond Block: &b{DIAMOND_BLOCK}",
    "&7Grass Block: &b{GRASS_BLOCK}",
    "&7Gold Block: &b{GOLD_BLOCK}",
    "&7Iron Block: &b{IRON_BLOCK}",
    "&7Lapis Block: &b{LAPIS_BLOCK}",
    "&7Coal Block: &b{COAL_BLOCK}"
  ],
  "commandTopPageSize": 5,
  "disableMobDamageWhenIslandVisitor": true,
  "islandTopCalcPeriodTicks": 18000,
  "islandTopManualCalcCooldownMiliseconds": 300000,
  "autoCalcIslands": true,
  "islandTopBroadcastMessage": true,
  "islandTopBroadcastMessageStart": "&7Starting IslandTOP Calculation.",
  "islandTopBroadcastMessageEnd": "&7Finished Calculation of %1$s islands in %2$s.",
  "islandSaveTaskPeriodTicks": 36000,
  "islandSaveBroadcastMessage": true,
  "islandSaveBroadcastMessageStart": "&7Saving Data...",
  "islandSaveBroadcastMessageEnd": "&7Finished Saving data ( %1$s ).",
  "numberFormatLocale": "en_US",
  "generatorProbability": {
    "1": [
      {
        "value": "COBBLESTONE",
        "weight": 5
      },
      {
        "value": "IRON_ORE",
        "weight": 1
      },
      {
        "value": "COAL_ORE",
        "weight": 3
      }
    ],
    "2": [
      {
        "value": "COBBLESTONE",
        "weight": 3
      },
      {
        "value": "GOLD_ORE",
        "weight": 2
      },
      {
        "value": "IRON_ORE",
        "weight": 2
      },
      {
        "value": "COAL_ORE",
        "weight": 3
      },
      {
        "value": "LAPIS_ORE",
        "weight": 1
      },
      {
        "value": "DIAMOND_ORE",
        "weight": 1
      }
    ],
    "3": [
      {
        "value": "COBBLESTONE",
        "weight": 3
      },
      {
        "value": "GOLD_ORE",
        "weight": 2
      },
      {
        "value": "IRON_ORE",
        "weight": 2
      },
      {
        "value": "COAL_ORE",
        "weight": 3
      },
      {
        "value": "LAPIS_ORE",
        "weight": 1
      },
      {
        "value": "DIAMOND_ORE",
        "weight": 1
      }
    ]
  },
  "islandMemberGUITitle": "&7Select a member.",
  "islandMemberGUIRows": 3,
  "islandMemberGUIBackgroundItem": {
    "material": "GRAY_STAINED_GLASS_PANE",
    "name": "&7",
    "lore": [
      ""
    ],
    "amt": 1
  },
  "islandMemberGUIHeadSlots": [
    10,
    13,
    16
  ],
  "islandMemberGUIItemMeta": {
    "name": "&b&l{player}",
    "lore": [
      "&7Click for more info"
    ]
  },
  "islandMemberGUINoMemberName": "&b&lInvite Another Island Member!",
  "islandMemberGUINoMemberLore": [
    "&7Invite another island member to manage them.",
    "&7Format: &b/is members invite <player>"
  ],
  "islandMemberShowMenu": true,
  "islandMemberActionGUITitle": "&b&l{player}",
  "islandMemberActionGUIBackgroundItem": {
    "material": "GRAY_STAINED_GLASS_PANE",
    "name": "&7",
    "lore": [
      ""
    ],
    "amt": 1
  },
  "islandMemberActionGUIRows": 3,
  "islandMemberActionItems": [
    {
      "guiItem": {
        "material": "PLAYER_HEAD",
        "name": "&bBack",
        "lore": [
          "&7Click to go back."
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is member"
      ],
      "slot": 0
    },
    {
      "guiItem": {
        "material": "BARRIER",
        "name": "&7Kick &b&l{player}",
        "lore": [
          "&7Click to kick"
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is members kick {player}"
      ],
      "slot": 10
    },
    {
      "guiItem": {
        "material": "DIAMOND_SWORD",
        "name": "&7Kick &b&l{player}",
        "lore": [
          "&7Click to kick"
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is members kick {player}"
      ],
      "slot": 13
    },
    {
      "guiItem": {
        "material": "GOLDEN_APPLE",
        "name": "&7Promote &b&l{player}&7 to leader",
        "lore": [
          "&7The current leader &b&lWILL &7lose their position",
          "&7Click to promote"
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is members promote {player}"
      ],
      "slot": 16
    }
  ],
  "islandBorderGUITitle": "&7Change border color",
  "islandBorderGUIRows": 3,
  "islandBorderGUIBackgroundItem": {
    "material": "GRAY_STAINED_GLASS_PANE",
    "name": "&7",
    "lore": [
      ""
    ],
    "amt": 1
  },
  "islandBorderGUIItems": {
    "RED": {
      "slot": 10,
      "displayItem": {
        "material": "RED_STAINED_GLASS",
        "name": "&cRed Border",
        "lore": [],
        "amt": 1
      }
    },
    "GREEN": {
      "slot": 12,
      "displayItem": {
        "material": "LIME_STAINED_GLASS",
        "name": "&aGreen Border",
        "lore": [],
        "amt": 1
      }
    },
    "BLUE": {
      "slot": 14,
      "displayItem": {
        "material": "LIGHT_BLUE_STAINED_GLASS",
        "name": "&bBlue Border",
        "lore": [],
        "amt": 1
      }
    },
    "NONE": {
      "slot": 16,
      "displayItem": {
        "material": "GLASS",
        "name": "&fNo Border",
        "lore": [],
        "amt": 1
      }
    }
  },
  "islandMenuGUITitle": "Island Menu",
  "islandMenuGUIRows": 3,
  "islandMenuGUIBackgroundItem": {
    "material": "GRAY_STAINED_GLASS_PANE",
    "name": "&9",
    "lore": [
      ""
    ],
    "amt": 1
  },
  "islandMenuGUIItems": [
    {
      "guiItem": {
        "material": "GRASS_BLOCK",
        "name": "&bGo to island",
        "lore": [
          "&7Click to go to island"
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is go"
      ],
      "slot": 10
    },
    {
      "guiItem": {
        "material": "BOOK",
        "name": "&bIsland Quests",
        "lore": [
          "&7Click to open quests"
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is quest"
      ],
      "slot": 13
    },
    {
      "guiItem": {
        "material": "PLAYER_HEAD",
        "name": "&bManage Members",
        "lore": [
          "&7Click to manage island members"
        ],
        "amt": 1
      },
      "commandsToExecute": [
        "is members"
      ],
      "slot": 16
    }
  ],
  "islandCreateGUITitle": "Choose an island!",
  "islandCreateGUIRows": 1,
  "islandCreateGUIBackgroundItem": {
    "material": "BLACK_STAINED_GLASS_PANE",
    "name": "&9",
    "lore": [
      ""
    ],
    "amt": 1
  },
  "islandCreateGUIIslandTypes": [
    {
      "name": "normal",
      "requirementPermission": "skyblockx.islands.default",
      "guiIndex": 2,
      "item": {
        "material": "GRASS_BLOCK",
        "name": "&aBasic Island",
        "lore": [
          "&aThis is the basic starter island",
          "&aComes with everything you need to get started."
        ],
        "amt": 1
      },
      "structureFile": "island.structure",
      "netherFile": "nether-island.structure"
    },
    {
      "name": "bedrock",
      "requirementPermission": "skyblockx.islands.bedrock",
      "guiIndex": 6,
      "item": {
        "material": "BEDROCK",
        "name": "&aBedrock Island",
        "lore": [
          "&aThis is the basic starter island",
          "&aComes with everything you need to get started."
        ],
        "amt": 1
      },
      "structureFile": "island.structure",
      "netherFile": "nether-island.structure"
    }
  ],
  "removeBlocksOnIslandDelete": false
}
```
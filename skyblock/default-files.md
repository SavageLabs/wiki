---
title: SkyblockX Default Files
description: 
published: 1
date: 2020-05-04T18:58:39.081Z
tags: default files, skyblockx
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
<h2>message.json</h2>

```json{
  "messagePrefix": "&7[&b!&7] ",
  "islandCreationMessage": "&7Island created with size %1$s.",
  "commandRequirementsNotAPlayer": "&cThis command requires the executor to be a player.",
  "commandRequirementsNotAnIslandMember": "&cThis command requires the executor to be a island member, create one using \"/is create\".",
  "commandRequirementsNotAnIslandLeader": "&cThis command requires the executor to be an island leader.",
  "commandRequirementsPlayerDoesNotHavePermission": "&cThis command requires the permission %1$s",
  "commandHelpGeneratorPageInvalid": "&cThe page %1$s does not exist.",
  "commandHelpGeneratorFormat": "&b/%1$s %2$s &8> &7 %3$s",
  "commandHelpGeneratorBackgroundColor": "GRAY",
  "commandHelpGeneratorNotRequired": "&cNo&r",
  "commandHelpGeneratorRequires": "&aYes&r",
  "commandHelpGeneratorIslandRequired": "&7Island member requirement: %1$s",
  "commandHelpGeneratorClickMeToPaste": "&7Click me to autocomplete.",
  "commandHelpGeneratorPageNavBack": "&b<<<",
  "commandHelpGeneratorPageNavNext": "&b>>>",
  "commandParsingArgIsNotInt": "&cThis argument is not an integer, please make it one.",
  "commandParsingPlayerDoesNotExist": "&cThis player does not exist.",
  "commandParsingArgIsNotBoolean": "&cThis argument is not a boolean, please make it 'true' or 'false'",
  "commandParsingPlayerIsYou": "&cYou cannot reference yourself.",
  "genericCommandsTooFewArgs": "&cThis command requires more arguments.",
  "genericCommandsTooManyArgs": "&cThis command requires less arguments.",
  "genericActionRequiresPermission": "&cThis action requires the permission %1$s",
  "genericCannotReferenceYourSelf": "&cYou cannot reference yourself.",
  "genericPlayerNotAnIslandMember": "&cThis player is not an island member.",
  "commandBaseHelp": "&7The base command for skyblock.",
  "commandSkyblockBaseHelp": "&7The base admin command for skyblock.",
  "commandBaseHelpMessage": "&aPlease execute /is help.",
  "commandSkyblockBaseHelpMessage": "&aPlease execute /sb help",
  "commandCreateCLIHeader": "&7&m-------&r &bIsland Types &7&m-------",
  "commandCreateCLIFormat": "&7%1$s. &b%2$s",
  "commandCreateCLIFormatTooltip": "&7Click to paste &b/is create %1$s&7 into your chatbar.",
  "commandCreateHelp": "&7Creates a skyblock island.",
  "commandCreateAlreadyHaveAnIsland": "&7You already have an island, use /is delete to delete your island.",
  "commandCreateSuccess": "&7Your island was successfully created.",
  "commandCreateCooldown": "&7Island Creation is on cooldown: &b%1$s &7seconds left.",
  "commandWorthHelp": "&7View island worth and level.",
  "commandWorthValue": "&7Your island value is &b$%1$s&7.",
  "commandWorthLevel": "&7Your island level based off of your worth is Lv. &b%1$s&7.",
  "commandChestHelp": "&7Open the island's virtual chest.",
  "commandChestOpening": "&7Opening the island chest.",
  "commandGoHelp": "&7Takes you to an island.",
  "commandGoTeleporting": "&7Taking you to your island...",
  "commandGoSetHelp": "&7Set the go point for the island.",
  "commandGoSetYouMustBeOnYourIsland": "&7You must be on your island to execute this command.",
  "commandGoSetSuccess": "&7You have successfully updated your &b/is go&7 location.",
  "commandDeleteHelp": "&7Deletes an island.",
  "commandDeleteDeletedIsland": "&7Your island has been deleted.",
  "commandSEPostionHelp": "&7Positions for skyblock edit.",
  "commandSEPosition": "&7Please right click a block to set it to position %1$s.",
  "commandSEPositionInvalidIndex": "&7The specified position index is invalid, it must be either 1 or 2.",
  "skyblockEditPositionSet": "&7You have set position %1$s to %2$s",
  "skyblockEditErrorPositionsNotInSameWorld": "&7Position 1 and position 2 are no in the same world.",
  "skyblockEditStructureSaved": "&7You have saved a structure to a file called %1$s",
  "commandSESaveStructureHelp": "&7Saves a structure to a specified file.",
  "commandSESaveStructurePositionsNotSet": "You have not set both positions use the command \"/is pos\" to set the positions.",
  "commandSEPasteStructurePasted": "&7Structure pasted successfully.",
  "commandBypassHelp": "&7Bypass island checks.",
  "commandBypassToggle": "&7You are now %1$s bypass mode.",
  "commandTopHelp": "&7Gets island top info.",
  "commandTopInvalidPage": "&7Invalid page",
  "commandTopIndexTooHigh": "&7This page does not exist.",
  "commandTopNotCalculated": "&7Island values have not been calculated yet. Run &b/sbx calc&7 to force calculation.",
  "commandCoopHelp": "&7Set another player to co-op mode.",
  "commandCoopInvokerSuccess": "&7You have added %1$s to your island as co-op",
  "commandCoopMessageRecipient": "&7You have been added as a co-op player to %1$s's island.",
  "commandCoopAuthorized": "&b%1$s&7 has been authorized as a co-op player; Once &b%2$s &7logs out, &b%1$s's&7 co-op status will be removed.",
  "commandCoopLoggedOut": "&7Your co-op access has expired because the player that authorized you logged out.",
  "commandCoopCannotHaveMoreCoopPlayers": "You cannot have more co-op players, run &c/is coop&r to view current co-op players, and remove them using &c/is remove <player>.",
  "commandHomeListHeader": "&7&m-------&r &bHomes &7&m-------",
  "commandHomeListFormat": "&7&b%1$s. &7%2$s",
  "commandHomeListRemoveTooltip": "&7Click to go!",
  "commandHomeList": "&7List island homes.",
  "commandHomeSetHelp": "&7Set island homes.",
  "commandHomeRemoveHelp": "&7Remove homes.",
  "commandHomeGoHelp": "&7Go to your homes.",
  "commandHomeHelp": "&7Opens a list with home commands.",
  "commandHomeGoSuccess": "&7You have been teleported to &b%1$s.",
  "commandHomeHomeSet": "&7You have set this location to your &b%1$s&7 home.",
  "commandHomeSetNotInIsland": "&7This location is not inside of the island's boundaries.",
  "commandHomeCannotHaveMoreHomes": "&7You cannot have more homes set.",
  "commandHomeDoesNotExist": "&7This home does not exist.",
  "commandHomeRemoveSuccess": "&7The home &b%1$s&7 has been removed.",
  "commandCalcMessage": "&7Calculated Island.",
  "commandCalcCooldown": "&7You are trying to calculate the island value too often, Cooldown: &b%1$s seconds left.",
  "commandCalcHelp": "&7Calculate your own island's value.",
  "commandBorderHelp": "&7Change your border color.",
  "commandHelpHelp": "&7View information about other commands.",
  "commandSkyblockHelpHelp": "&7View other admin command info.",
  "commandRemoveHelp": "&7Removes island/co-op member.",
  "commandRemoveInvokerSuccess": "&7You have removed %1$s from your island.",
  "commandRemoveInvokerCoopRemoved": "&7%1$s's co-op status has been removed.",
  "commandRemoveInvokerPlayerNotOnIsland": "&7The specified player's location is currently not on your island.",
  "commandRemovedCoopStatus": "&7Your co-op status has been removed due to you being removed from the island.",
  "commandVisitHelp": "&7Teleport to islands of other players.",
  "commandVisitPossibleLocationsHeader": "&7You can teleport to the following locations...",
  "commandVisitPossibleLocationsFormat": "&7%1$s. &b%2$s's island.",
  "commandVisitThisIslandIsNotValid": "&7The player %1$s does not own an island. Type &b/is tp &r&7to list possible locations.",
  "commandVisitTeleporting": "&7Teleporting you to %1$s's island.",
  "commandVisitNoPermission": "&7The specified island does not have you as co-op, an island member, or allow visitors.",
  "commandJoinHelp": "&7Join an island.",
  "commandJoinNotInvited": "&7You have not been invited to %1$s's island.",
  "commandJoinSuccess": "&7You have joined %1$s's island.",
  "commandJoinHaveIsland": "&7You already have an island.",
  "commandQuestHelp": "&7View Quest GUI.",
  "commandReloadHelp": "&7Reloads the skyblock config files.",
  "commandReloadSuccess": "&7Reloaded configs and saved data.",
  "commandMenuHelp": "&7Opens the Island Menu GUI.",
  "islandCreateGUIYouDontHavePermission": "You do not have permission to use this island.",
  "commandMemberInviteHelp": "invite a member to your island",
  "commandMemberInviteSuccess": "&7You have invited %1$s to your island.",
  "commandMemberInviteMessage": "&7%1$s has invited you to their island, click to accept!",
  "commandMemberInviteLimit": "&7You cannot invite more members to your island, the limit is %1$s.",
  "commandMemberKickHelp": "&7Remove member from island.",
  "commandMemberKickLimit": "&7There are no members to remove!",
  "commandMemberKickNotFound": "&7Your island does not have this member, names are &cCase Sensitive!",
  "commandMemberKicked": "&7You have successfully removed %1$s from your island.",
  "commandMemberPromoteHelp": "&7Promote a member to leader.",
  "commandMemberNoMembers": "&7Your island does not have any members to promote.",
  "commandMemberPromoteNotFound": "&7Your island does not have this member, names are &cCase Sensitive!",
  "commandMemberPromotedSuccess": "&b%1$s&7 was promoted to leader.",
  "commandMemberPromoteYouHaveBeenPromoted": "&7You have been promoted to &bisland leader&7.",
  "commandMemberListHelp": "&7List all the members.",
  "commandMemberListHeader": "&7&m-------&r &bMembers &7&m-------",
  "commandMemberListFormat": "&7&b%1$s. &7%2$s",
  "commandMemberListRemoveTooltip": "&7Click to remove!",
  "commandMemberHelp": "&7Member commands.",
  "commandMemberAlreadyPartOfIsland": "&7This player is already in your island",
  "commandLeaveHelp": "&7Leave your island.",
  "commandLeaveSuccess": "&7You have successfully left your island.",
  "commandLeaveMemberLeftIsland": "&7%1$s has left your island.",
  "commandLeaveDeniedLeader": "&7You cannot leave an island as a leader, promote someone else to leader, or delete it.",
  "commandResetHelp": "&7Reset your island.",
  "commandValueHelp": "&7Get the monetary value of a block you're holding.",
  "commandValueInfo": "&7The value of this block is &b%1$s",
  "commandSkyblockOpenChestHelp": "Open an island chest.",
  "commandSkyblockOpenChestNotAnIslandMember": "&7This player is &bnot&7 an island member.",
  "commandSkyblockOpenChestOpening": "&7Opening target island's chest...",
  "commandSkyblockRemoveHelp": "&7Delete a player's island.",
  "commandSkyblockRemoveSuccess": "&7The island was successfully deleted.",
  "commandSkyblockRemoveNotAnIslandOwner": "&7This player is &bnot&7 an island owner.",
  "commandSkyblockKickHelp": "&7Kick a player from their island.",
  "commandSkyblockKickMemberKicked": "&b%1$s was kicked from their island.",
  "commandSkyblockKickMemberKickedOwner": "&b%1$s is now the owner of the island.",
  "commandSkyblockKickIslandDeleted": "&7The island has been deleted since the island has no members left to inherit the island.",
  "commandSkyblockNewOwnerHelp": "&7Set a new owner for an island.",
  "commandSkyblockNewOwnerSuccess": "&7New owner successfully set.",
  "commandSkyblockCalcHelp": "&7Calculates every island's price.",
  "commandSkyblockCalcDone": "&7Calculated %1$s islands.",
  "commandSkyblockCalcStart": "&7Starting Calculation...",
  "commandAllowVisitorsHelp": "&7Allow visitors to your island using /is teleport <owner-name>.",
  "commandAllowVisitorsStatus": "&7Your visitor allowed status is now set to &b%1$s&7.",
  "commandBiomeHelp": "&7Change your island's biome.",
  "commandBiomeSuccess": "&7You have changed your island's biome to %1$s, you need to re-log to see changes.",
  "commandBiomeInvalidBiome": "&7The specified biome is invalid.",
  "listenerVoidDeathPrevented": "&7You fell into the void, teleporting you back.",
  "listenerDeathTeleport": "&7You've been teleported to your island.",
  "listenerBlockPlacementDenied": "&7You can only place blocks inside of your island.",
  "listenerActionDeniedCreateAnIslandFirst": "&7This action has been denied, please create an island first.",
  "listenerObsidianBucketLava": "&7The obsidian has been turned back to lava, be careful!",
  "listenerPlayerCannotInteract": "&7You cannot interact with this block.",
  "questActivationTrigger": "&7You have activated the quest &b{quest}",
  "questIsOneTimeAndAlreadyCompleted": "&7This quest is a onetime quest and is already completed.",
  "questOrderNoNextQuestWasFound": "&7No next quest was found.",
  "nextQuestMessage": "&7Your next quest is &b%1$s",
  "questInProgressPlaceholder": "&a&lIN PROGRESS",
  "questCompletedPlaceholder": "&b&lCOMPLETED",
  "questNotStarted": "&c&lNOT STARTED",
  "questProgressCompletedChar": "&b=",
  "questProgressInCompleteChar": "&7=",
  "questProgressBarMessage": "&b&l{quest-name} {progress-bar} &b{percentage}%",
  "islandNetherTeleported": "&7You have been teleported to your nether island.",
  "islandCreatedTitle": "&9SkyblockX",
  "islandCreatedSubtitle": "&7By: ProSavage"
}```

<h2>blockvalues.json</h2>

```json
{
  "blockValues": {
    "GRASS_BLOCK": 3.0,
    "DIRT": 1.0,
    "DIAMOND_BLOCK": 100.0,
    "GOLD_BLOCK": 50.0,
    "IRON_BLOCK": 25.0,
    "LAPIS_BLOCK": 20.0,
    "COAL_BLOCK": 10.0,
    "SPAWNER": 1000.0,
    "ACACIA_BOAT": 0.0,
    "ACACIA_BUTTON": 0.0,
    "ACACIA_DOOR": 0.0,
    "ACACIA_FENCE": 0.0,
    "ACACIA_FENCE_GATE": 0.0,
    "ACACIA_LEAVES": 0.0,
    "ACACIA_LOG": 0.0,
    "ACACIA_PLANKS": 0.0,
    "ACACIA_PRESSURE_PLATE": 0.0,
    "ACACIA_SAPLING": 0.0,
    "ACACIA_SIGN": 0.0,
    "ACACIA_SLAB": 0.0,
    "ACACIA_STAIRS": 0.0,
    "ACACIA_TRAPDOOR": 0.0,
    "ACACIA_WALL_SIGN": 0.0,
    "ACACIA_WOOD": 0.0,
    "ACTIVATOR_RAIL": 0.0,
    "AIR": 0.0,
    "ALLIUM": 0.0,
    "ANDESITE": 0.0,
    "ANDESITE_SLAB": 0.0,
    "ANDESITE_STAIRS": 0.0,
    "ANDESITE_WALL": 0.0,
    "ANVIL": 0.0,
    "APPLE": 0.0,
    "ARMOR_STAND": 0.0,
    "ARROW": 0.0,
    "ATTACHED_MELON_STEM": 0.0,
    "ATTACHED_PUMPKIN_STEM": 0.0,
    "AZURE_BLUET": 0.0,
    "BAKED_POTATO": 0.0,
    "BAMBOO": 0.0,
    "BAMBOO_SAPLING": 0.0,
    "BARREL": 0.0,
    "BARRIER": 0.0,
    "BAT_SPAWN_EGG": 0.0,
    "BEACON": 0.0,
    "BEDROCK": 0.0,
    "BEEF": 0.0,
    "BEEHIVE": 0.0,
    "BEETROOT": 0.0,
    "BEETROOTS": 0.0,
    "BEETROOT_SEEDS": 0.0,
    "BEETROOT_SOUP": 0.0,
    "BEE_NEST": 0.0,
    "BEE_SPAWN_EGG": 0.0,
    "BELL": 0.0,
    "BIRCH_BOAT": 0.0,
    "BIRCH_BUTTON": 0.0,
    "BIRCH_DOOR": 0.0,
    "BIRCH_FENCE": 0.0,
    "BIRCH_FENCE_GATE": 0.0,
    "BIRCH_LEAVES": 0.0,
    "BIRCH_LOG": 0.0,
    "BIRCH_PLANKS": 0.0,
    "BIRCH_PRESSURE_PLATE": 0.0,
    "BIRCH_SAPLING": 0.0,
    "BIRCH_SIGN": 0.0,
    "BIRCH_SLAB": 0.0,
    "BIRCH_STAIRS": 0.0,
    "BIRCH_TRAPDOOR": 0.0,
    "BIRCH_WALL_SIGN": 0.0,
    "BIRCH_WOOD": 0.0,
    "BLACK_BANNER": 0.0,
    "BLACK_BED": 0.0,
    "BLACK_CARPET": 0.0,
    "BLACK_CONCRETE": 0.0,
    "BLACK_CONCRETE_POWDER": 0.0,
    "BLACK_DYE": 0.0,
    "BLACK_GLAZED_TERRACOTTA": 0.0,
    "BLACK_SHULKER_BOX": 0.0,
    "BLACK_STAINED_GLASS": 0.0,
    "BLACK_STAINED_GLASS_PANE": 0.0,
    "BLACK_TERRACOTTA": 0.0,
    "BLACK_WALL_BANNER": 0.0,
    "BLACK_WOOL": 0.0,
    "BLAST_FURNACE": 0.0,
    "BLAZE_POWDER": 0.0,
    "BLAZE_ROD": 0.0,
    "BLAZE_SPAWN_EGG": 0.0,
    "BLUE_BANNER": 0.0,
    "BLUE_BED": 0.0,
    "BLUE_CARPET": 0.0,
    "BLUE_CONCRETE": 0.0,
    "BLUE_CONCRETE_POWDER": 0.0,
    "BLUE_DYE": 0.0,
    "BLUE_GLAZED_TERRACOTTA": 0.0,
    "BLUE_ICE": 0.0,
    "BLUE_ORCHID": 0.0,
    "BLUE_SHULKER_BOX": 0.0,
    "BLUE_STAINED_GLASS": 0.0,
    "BLUE_STAINED_GLASS_PANE": 0.0,
    "BLUE_TERRACOTTA": 0.0,
    "BLUE_WALL_BANNER": 0.0,
    "BLUE_WOOL": 0.0,
    "BONE": 0.0,
    "BONE_BLOCK": 0.0,
    "BONE_MEAL": 0.0,
    "BOOK": 0.0,
    "BOOKSHELF": 0.0,
    "BOW": 0.0,
    "BOWL": 0.0,
    "BRAIN_CORAL": 0.0,
    "BRAIN_CORAL_BLOCK": 0.0,
    "BRAIN_CORAL_FAN": 0.0,
    "BRAIN_CORAL_WALL_FAN": 0.0,
    "BREAD": 0.0,
    "BREWING_STAND": 0.0,
    "BRICK": 0.0,
    "BRICKS": 0.0,
    "BRICK_SLAB": 0.0,
    "BRICK_STAIRS": 0.0,
    "BRICK_WALL": 0.0,
    "BROWN_BANNER": 0.0,
    "BROWN_BED": 0.0,
    "BROWN_CARPET": 0.0,
    "BROWN_CONCRETE": 0.0,
    "BROWN_CONCRETE_POWDER": 0.0,
    "BROWN_DYE": 0.0,
    "BROWN_GLAZED_TERRACOTTA": 0.0,
    "BROWN_MUSHROOM": 0.0,
    "BROWN_MUSHROOM_BLOCK": 0.0,
    "BROWN_SHULKER_BOX": 0.0,
    "BROWN_STAINED_GLASS": 0.0,
    "BROWN_STAINED_GLASS_PANE": 0.0,
    "BROWN_TERRACOTTA": 0.0,
    "BROWN_WALL_BANNER": 0.0,
    "BROWN_WOOL": 0.0,
    "BUBBLE_COLUMN": 0.0,
    "BUBBLE_CORAL": 0.0,
    "BUBBLE_CORAL_BLOCK": 0.0,
    "BUBBLE_CORAL_FAN": 0.0,
    "BUBBLE_CORAL_WALL_FAN": 0.0,
    "BUCKET": 0.0,
    "CACTUS": 0.0,
    "CAKE": 0.0,
    "CAMPFIRE": 0.0,
    "CARROT": 0.0,
    "CARROTS": 0.0,
    "CARROT_ON_A_STICK": 0.0,
    "CARTOGRAPHY_TABLE": 0.0,
    "CARVED_PUMPKIN": 0.0,
    "CAT_SPAWN_EGG": 0.0,
    "CAULDRON": 0.0,
    "CAVE_AIR": 0.0,
    "CAVE_SPIDER_SPAWN_EGG": 0.0,
    "CHAINMAIL_BOOTS": 0.0,
    "CHAINMAIL_CHESTPLATE": 0.0,
    "CHAINMAIL_HELMET": 0.0,
    "CHAINMAIL_LEGGINGS": 0.0,
    "CHAIN_COMMAND_BLOCK": 0.0,
    "CHARCOAL": 0.0,
    "CHEST": 0.0,
    "CHEST_MINECART": 0.0,
    "CHICKEN": 0.0,
    "CHICKEN_SPAWN_EGG": 0.0,
    "CHIPPED_ANVIL": 0.0,
    "CHISELED_QUARTZ_BLOCK": 0.0,
    "CHISELED_RED_SANDSTONE": 0.0,
    "CHISELED_SANDSTONE": 0.0,
    "CHISELED_STONE_BRICKS": 0.0,
    "CHORUS_FLOWER": 0.0,
    "CHORUS_FRUIT": 0.0,
    "CHORUS_PLANT": 0.0,
    "CLAY": 0.0,
    "CLAY_BALL": 0.0,
    "CLOCK": 0.0,
    "COAL": 0.0,
    "COAL_ORE": 0.0,
    "COARSE_DIRT": 0.0,
    "COBBLESTONE": 0.0,
    "COBBLESTONE_SLAB": 0.0,
    "COBBLESTONE_STAIRS": 0.0,
    "COBBLESTONE_WALL": 0.0,
    "COBWEB": 0.0,
    "COCOA": 0.0,
    "COCOA_BEANS": 0.0,
    "COD": 0.0,
    "COD_BUCKET": 0.0,
    "COD_SPAWN_EGG": 0.0,
    "COMMAND_BLOCK": 0.0,
    "COMMAND_BLOCK_MINECART": 0.0,
    "COMPARATOR": 0.0,
    "COMPASS": 0.0,
    "COMPOSTER": 0.0,
    "CONDUIT": 0.0,
    "COOKED_BEEF": 0.0,
    "COOKED_CHICKEN": 0.0,
    "COOKED_COD": 0.0,
    "COOKED_MUTTON": 0.0,
    "COOKED_PORKCHOP": 0.0,
    "COOKED_RABBIT": 0.0,
    "COOKED_SALMON": 0.0,
    "COOKIE": 0.0,
    "CORNFLOWER": 0.0,
    "COW_SPAWN_EGG": 0.0,
    "CRACKED_STONE_BRICKS": 0.0,
    "CRAFTING_TABLE": 0.0,
    "CREEPER_BANNER_PATTERN": 0.0,
    "CREEPER_HEAD": 0.0,
    "CREEPER_SPAWN_EGG": 0.0,
    "CREEPER_WALL_HEAD": 0.0,
    "CROSSBOW": 0.0,
    "CUT_RED_SANDSTONE": 0.0,
    "CUT_RED_SANDSTONE_SLAB": 0.0,
    "CUT_SANDSTONE": 0.0,
    "CUT_SANDSTONE_SLAB": 0.0,
    "CYAN_BANNER": 0.0,
    "CYAN_BED": 0.0,
    "CYAN_CARPET": 0.0,
    "CYAN_CONCRETE": 0.0,
    "CYAN_CONCRETE_POWDER": 0.0,
    "CYAN_DYE": 0.0,
    "CYAN_GLAZED_TERRACOTTA": 0.0,
    "CYAN_SHULKER_BOX": 0.0,
    "CYAN_STAINED_GLASS": 0.0,
    "CYAN_STAINED_GLASS_PANE": 0.0,
    "CYAN_TERRACOTTA": 0.0,
    "CYAN_WALL_BANNER": 0.0,
    "CYAN_WOOL": 0.0,
    "DAMAGED_ANVIL": 0.0,
    "DANDELION": 0.0,
    "DARK_OAK_BOAT": 0.0,
    "DARK_OAK_BUTTON": 0.0,
    "DARK_OAK_DOOR": 0.0,
    "DARK_OAK_FENCE": 0.0,
    "DARK_OAK_FENCE_GATE": 0.0,
    "DARK_OAK_LEAVES": 0.0,
    "DARK_OAK_LOG": 0.0,
    "DARK_OAK_PLANKS": 0.0,
    "DARK_OAK_PRESSURE_PLATE": 0.0,
    "DARK_OAK_SAPLING": 0.0,
    "DARK_OAK_SIGN": 0.0,
    "DARK_OAK_SLAB": 0.0,
    "DARK_OAK_STAIRS": 0.0,
    "DARK_OAK_TRAPDOOR": 0.0,
    "DARK_OAK_WALL_SIGN": 0.0,
    "DARK_OAK_WOOD": 0.0,
    "DARK_PRISMARINE": 0.0,
    "DARK_PRISMARINE_SLAB": 0.0,
    "DARK_PRISMARINE_STAIRS": 0.0,
    "DAYLIGHT_DETECTOR": 0.0,
    "DEAD_BRAIN_CORAL": 0.0,
    "DEAD_BRAIN_CORAL_BLOCK": 0.0,
    "DEAD_BRAIN_CORAL_FAN": 0.0,
    "DEAD_BRAIN_CORAL_WALL_FAN": 0.0,
    "DEAD_BUBBLE_CORAL": 0.0,
    "DEAD_BUBBLE_CORAL_BLOCK": 0.0,
    "DEAD_BUBBLE_CORAL_FAN": 0.0,
    "DEAD_BUBBLE_CORAL_WALL_FAN": 0.0,
    "DEAD_BUSH": 0.0,
    "DEAD_FIRE_CORAL": 0.0,
    "DEAD_FIRE_CORAL_BLOCK": 0.0,
    "DEAD_FIRE_CORAL_FAN": 0.0,
    "DEAD_FIRE_CORAL_WALL_FAN": 0.0,
    "DEAD_HORN_CORAL": 0.0,
    "DEAD_HORN_CORAL_BLOCK": 0.0,
    "DEAD_HORN_CORAL_FAN": 0.0,
    "DEAD_HORN_CORAL_WALL_FAN": 0.0,
    "DEAD_TUBE_CORAL": 0.0,
    "DEAD_TUBE_CORAL_BLOCK": 0.0,
    "DEAD_TUBE_CORAL_FAN": 0.0,
    "DEAD_TUBE_CORAL_WALL_FAN": 0.0,
    "DEBUG_STICK": 0.0,
    "DETECTOR_RAIL": 0.0,
    "DIAMOND": 0.0,
    "DIAMOND_AXE": 0.0,
    "DIAMOND_BOOTS": 0.0,
    "DIAMOND_CHESTPLATE": 0.0,
    "DIAMOND_HELMET": 0.0,
    "DIAMOND_HOE": 0.0,
    "DIAMOND_HORSE_ARMOR": 0.0,
    "DIAMOND_LEGGINGS": 0.0,
    "DIAMOND_ORE": 0.0,
    "DIAMOND_PICKAXE": 0.0,
    "DIAMOND_SHOVEL": 0.0,
    "DIAMOND_SWORD": 0.0,
    "DIORITE": 0.0,
    "DIORITE_SLAB": 0.0,
    "DIORITE_STAIRS": 0.0,
    "DIORITE_WALL": 0.0,
    "DISPENSER": 0.0,
    "DOLPHIN_SPAWN_EGG": 0.0,
    "DONKEY_SPAWN_EGG": 0.0,
    "DRAGON_BREATH": 0.0,
    "DRAGON_EGG": 0.0,
    "DRAGON_HEAD": 0.0,
    "DRAGON_WALL_HEAD": 0.0,
    "DRIED_KELP": 0.0,
    "DRIED_KELP_BLOCK": 0.0,
    "DROPPER": 0.0,
    "DROWNED_SPAWN_EGG": 0.0,
    "EGG": 0.0,
    "ELDER_GUARDIAN_SPAWN_EGG": 0.0,
    "ELYTRA": 0.0,
    "EMERALD": 0.0,
    "EMERALD_BLOCK": 0.0,
    "EMERALD_ORE": 0.0,
    "ENCHANTED_BOOK": 0.0,
    "ENCHANTED_GOLDEN_APPLE": 0.0,
    "ENCHANTING_TABLE": 0.0,
    "ENDERMAN_SPAWN_EGG": 0.0,
    "ENDERMITE_SPAWN_EGG": 0.0,
    "ENDER_CHEST": 0.0,
    "ENDER_EYE": 0.0,
    "ENDER_PEARL": 0.0,
    "END_CRYSTAL": 0.0,
    "END_GATEWAY": 0.0,
    "END_PORTAL": 0.0,
    "END_PORTAL_FRAME": 0.0,
    "END_ROD": 0.0,
    "END_STONE": 0.0,
    "END_STONE_BRICKS": 0.0,
    "END_STONE_BRICK_SLAB": 0.0,
    "END_STONE_BRICK_STAIRS": 0.0,
    "END_STONE_BRICK_WALL": 0.0,
    "EVOKER_SPAWN_EGG": 0.0,
    "EXPERIENCE_BOTTLE": 0.0,
    "FARMLAND": 0.0,
    "FEATHER": 0.0,
    "FERMENTED_SPIDER_EYE": 0.0,
    "FERN": 0.0,
    "FILLED_MAP": 0.0,
    "FIRE": 0.0,
    "FIREWORK_ROCKET": 0.0,
    "FIREWORK_STAR": 0.0,
    "FIRE_CHARGE": 0.0,
    "FIRE_CORAL": 0.0,
    "FIRE_CORAL_BLOCK": 0.0,
    "FIRE_CORAL_FAN": 0.0,
    "FIRE_CORAL_WALL_FAN": 0.0,
    "FISHING_ROD": 0.0,
    "FLETCHING_TABLE": 0.0,
    "FLINT": 0.0,
    "FLINT_AND_STEEL": 0.0,
    "FLOWER_BANNER_PATTERN": 0.0,
    "FLOWER_POT": 0.0,
    "FOX_SPAWN_EGG": 0.0,
    "FROSTED_ICE": 0.0,
    "FURNACE": 0.0,
    "FURNACE_MINECART": 0.0,
    "GHAST_SPAWN_EGG": 0.0,
    "GHAST_TEAR": 0.0,
    "GLASS": 0.0,
    "GLASS_BOTTLE": 0.0,
    "GLASS_PANE": 0.0,
    "GLISTERING_MELON_SLICE": 0.0,
    "GLOBE_BANNER_PATTERN": 0.0,
    "GLOWSTONE": 0.0,
    "GLOWSTONE_DUST": 0.0,
    "GOLDEN_APPLE": 0.0,
    "GOLDEN_AXE": 0.0,
    "GOLDEN_BOOTS": 0.0,
    "GOLDEN_CARROT": 0.0,
    "GOLDEN_CHESTPLATE": 0.0,
    "GOLDEN_HELMET": 0.0,
    "GOLDEN_HOE": 0.0,
    "GOLDEN_HORSE_ARMOR": 0.0,
    "GOLDEN_LEGGINGS": 0.0,
    "GOLDEN_PICKAXE": 0.0,
    "GOLDEN_SHOVEL": 0.0,
    "GOLDEN_SWORD": 0.0,
    "GOLD_INGOT": 0.0,
    "GOLD_NUGGET": 0.0,
    "GOLD_ORE": 0.0,
    "GRANITE": 0.0,
    "GRANITE_SLAB": 0.0,
    "GRANITE_STAIRS": 0.0,
    "GRANITE_WALL": 0.0,
    "GRASS": 0.0,
    "GRASS_PATH": 0.0,
    "GRAVEL": 0.0,
    "GRAY_BANNER": 0.0,
    "GRAY_BED": 0.0,
    "GRAY_CARPET": 0.0,
    "GRAY_CONCRETE": 0.0,
    "GRAY_CONCRETE_POWDER": 0.0,
    "GRAY_DYE": 0.0,
    "GRAY_GLAZED_TERRACOTTA": 0.0,
    "GRAY_SHULKER_BOX": 0.0,
    "GRAY_STAINED_GLASS": 0.0,
    "GRAY_STAINED_GLASS_PANE": 0.0,
    "GRAY_TERRACOTTA": 0.0,
    "GRAY_WALL_BANNER": 0.0,
    "GRAY_WOOL": 0.0,
    "GREEN_BANNER": 0.0,
    "GREEN_BED": 0.0,
    "GREEN_CARPET": 0.0,
    "GREEN_CONCRETE": 0.0,
    "GREEN_CONCRETE_POWDER": 0.0,
    "GREEN_DYE": 0.0,
    "GREEN_GLAZED_TERRACOTTA": 0.0,
    "GREEN_SHULKER_BOX": 0.0,
    "GREEN_STAINED_GLASS": 0.0,
    "GREEN_STAINED_GLASS_PANE": 0.0,
    "GREEN_TERRACOTTA": 0.0,
    "GREEN_WALL_BANNER": 0.0,
    "GREEN_WOOL": 0.0,
    "GRINDSTONE": 0.0,
    "GUARDIAN_SPAWN_EGG": 0.0,
    "GUNPOWDER": 0.0,
    "HAY_BLOCK": 0.0,
    "HEART_OF_THE_SEA": 0.0,
    "HEAVY_WEIGHTED_PRESSURE_PLATE": 0.0,
    "HONEYCOMB": 0.0,
    "HONEYCOMB_BLOCK": 0.0,
    "HONEY_BLOCK": 0.0,
    "HONEY_BOTTLE": 0.0,
    "HOPPER": 0.0,
    "HOPPER_MINECART": 0.0,
    "HORN_CORAL": 0.0,
    "HORN_CORAL_BLOCK": 0.0,
    "HORN_CORAL_FAN": 0.0,
    "HORN_CORAL_WALL_FAN": 0.0,
    "HORSE_SPAWN_EGG": 0.0,
    "HUSK_SPAWN_EGG": 0.0,
    "ICE": 0.0,
    "INFESTED_CHISELED_STONE_BRICKS": 0.0,
    "INFESTED_COBBLESTONE": 0.0,
    "INFESTED_CRACKED_STONE_BRICKS": 0.0,
    "INFESTED_MOSSY_STONE_BRICKS": 0.0,
    "INFESTED_STONE": 0.0,
    "INFESTED_STONE_BRICKS": 0.0,
    "INK_SAC": 0.0,
    "IRON_AXE": 0.0,
    "IRON_BARS": 0.0,
    "IRON_BOOTS": 0.0,
    "IRON_CHESTPLATE": 0.0,
    "IRON_DOOR": 0.0,
    "IRON_HELMET": 0.0,
    "IRON_HOE": 0.0,
    "IRON_HORSE_ARMOR": 0.0,
    "IRON_INGOT": 0.0,
    "IRON_LEGGINGS": 0.0,
    "IRON_NUGGET": 0.0,
    "IRON_ORE": 0.0,
    "IRON_PICKAXE": 0.0,
    "IRON_SHOVEL": 0.0,
    "IRON_SWORD": 0.0,
    "IRON_TRAPDOOR": 0.0,
    "ITEM_FRAME": 0.0,
    "JACK_O_LANTERN": 0.0,
    "JIGSAW": 0.0,
    "JUKEBOX": 0.0,
    "JUNGLE_BOAT": 0.0,
    "JUNGLE_BUTTON": 0.0,
    "JUNGLE_DOOR": 0.0,
    "JUNGLE_FENCE": 0.0,
    "JUNGLE_FENCE_GATE": 0.0,
    "JUNGLE_LEAVES": 0.0,
    "JUNGLE_LOG": 0.0,
    "JUNGLE_PLANKS": 0.0,
    "JUNGLE_PRESSURE_PLATE": 0.0,
    "JUNGLE_SAPLING": 0.0,
    "JUNGLE_SIGN": 0.0,
    "JUNGLE_SLAB": 0.0,
    "JUNGLE_STAIRS": 0.0,
    "JUNGLE_TRAPDOOR": 0.0,
    "JUNGLE_WALL_SIGN": 0.0,
    "JUNGLE_WOOD": 0.0,
    "KELP": 0.0,
    "KELP_PLANT": 0.0,
    "KNOWLEDGE_BOOK": 0.0,
    "LADDER": 0.0,
    "LANTERN": 0.0,
    "LAPIS_LAZULI": 0.0,
    "LAPIS_ORE": 0.0,
    "LARGE_FERN": 0.0,
    "LAVA": 0.0,
    "LAVA_BUCKET": 0.0,
    "LEAD": 0.0,
    "LEATHER": 0.0,
    "LEATHER_BOOTS": 0.0,
    "LEATHER_CHESTPLATE": 0.0,
    "LEATHER_HELMET": 0.0,
    "LEATHER_HORSE_ARMOR": 0.0,
    "LEATHER_LEGGINGS": 0.0,
    "LECTERN": 0.0,
    "LEVER": 0.0,
    "LIGHT_BLUE_BANNER": 0.0,
    "LIGHT_BLUE_BED": 0.0,
    "LIGHT_BLUE_CARPET": 0.0,
    "LIGHT_BLUE_CONCRETE": 0.0,
    "LIGHT_BLUE_CONCRETE_POWDER": 0.0,
    "LIGHT_BLUE_DYE": 0.0,
    "LIGHT_BLUE_GLAZED_TERRACOTTA": 0.0,
    "LIGHT_BLUE_SHULKER_BOX": 0.0,
    "LIGHT_BLUE_STAINED_GLASS": 0.0,
    "LIGHT_BLUE_STAINED_GLASS_PANE": 0.0,
    "LIGHT_BLUE_TERRACOTTA": 0.0,
    "LIGHT_BLUE_WALL_BANNER": 0.0,
    "LIGHT_BLUE_WOOL": 0.0,
    "LIGHT_GRAY_BANNER": 0.0,
    "LIGHT_GRAY_BED": 0.0,
    "LIGHT_GRAY_CARPET": 0.0,
    "LIGHT_GRAY_CONCRETE": 0.0,
    "LIGHT_GRAY_CONCRETE_POWDER": 0.0,
    "LIGHT_GRAY_DYE": 0.0,
    "LIGHT_GRAY_GLAZED_TERRACOTTA": 0.0,
    "LIGHT_GRAY_SHULKER_BOX": 0.0,
    "LIGHT_GRAY_STAINED_GLASS": 0.0,
    "LIGHT_GRAY_STAINED_GLASS_PANE": 0.0,
    "LIGHT_GRAY_TERRACOTTA": 0.0,
    "LIGHT_GRAY_WALL_BANNER": 0.0,
    "LIGHT_GRAY_WOOL": 0.0,
    "LIGHT_WEIGHTED_PRESSURE_PLATE": 0.0,
    "LILAC": 0.0,
    "LILY_OF_THE_VALLEY": 0.0,
    "LILY_PAD": 0.0,
    "LIME_BANNER": 0.0,
    "LIME_BED": 0.0,
    "LIME_CARPET": 0.0,
    "LIME_CONCRETE": 0.0,
    "LIME_CONCRETE_POWDER": 0.0,
    "LIME_DYE": 0.0,
    "LIME_GLAZED_TERRACOTTA": 0.0,
    "LIME_SHULKER_BOX": 0.0,
    "LIME_STAINED_GLASS": 0.0,
    "LIME_STAINED_GLASS_PANE": 0.0,
    "LIME_TERRACOTTA": 0.0,
    "LIME_WALL_BANNER": 0.0,
    "LIME_WOOL": 0.0,
    "LINGERING_POTION": 0.0,
    "LLAMA_SPAWN_EGG": 0.0,
    "LOOM": 0.0,
    "MAGENTA_BANNER": 0.0,
    "MAGENTA_BED": 0.0,
    "MAGENTA_CARPET": 0.0,
    "MAGENTA_CONCRETE": 0.0,
    "MAGENTA_CONCRETE_POWDER": 0.0,
    "MAGENTA_DYE": 0.0,
    "MAGENTA_GLAZED_TERRACOTTA": 0.0,
    "MAGENTA_SHULKER_BOX": 0.0,
    "MAGENTA_STAINED_GLASS": 0.0,
    "MAGENTA_STAINED_GLASS_PANE": 0.0,
    "MAGENTA_TERRACOTTA": 0.0,
    "MAGENTA_WALL_BANNER": 0.0,
    "MAGENTA_WOOL": 0.0,
    "MAGMA_BLOCK": 0.0,
    "MAGMA_CREAM": 0.0,
    "MAGMA_CUBE_SPAWN_EGG": 0.0,
    "MAP": 0.0,
    "MELON": 0.0,
    "MELON_SEEDS": 0.0,
    "MELON_SLICE": 0.0,
    "MELON_STEM": 0.0,
    "MILK_BUCKET": 0.0,
    "MINECART": 0.0,
    "MOJANG_BANNER_PATTERN": 0.0,
    "MOOSHROOM_SPAWN_EGG": 0.0,
    "MOSSY_COBBLESTONE": 0.0,
    "MOSSY_COBBLESTONE_SLAB": 0.0,
    "MOSSY_COBBLESTONE_STAIRS": 0.0,
    "MOSSY_COBBLESTONE_WALL": 0.0,
    "MOSSY_STONE_BRICKS": 0.0,
    "MOSSY_STONE_BRICK_SLAB": 0.0,
    "MOSSY_STONE_BRICK_STAIRS": 0.0,
    "MOSSY_STONE_BRICK_WALL": 0.0,
    "MOVING_PISTON": 0.0,
    "MULE_SPAWN_EGG": 0.0,
    "MUSHROOM_STEM": 0.0,
    "MUSHROOM_STEW": 0.0,
    "MUSIC_DISC_11": 0.0,
    "MUSIC_DISC_13": 0.0,
    "MUSIC_DISC_BLOCKS": 0.0,
    "MUSIC_DISC_CAT": 0.0,
    "MUSIC_DISC_CHIRP": 0.0,
    "MUSIC_DISC_FAR": 0.0,
    "MUSIC_DISC_MALL": 0.0,
    "MUSIC_DISC_MELLOHI": 0.0,
    "MUSIC_DISC_STAL": 0.0,
    "MUSIC_DISC_STRAD": 0.0,
    "MUSIC_DISC_WAIT": 0.0,
    "MUSIC_DISC_WARD": 0.0,
    "MUTTON": 0.0,
    "MYCELIUM": 0.0,
    "NAME_TAG": 0.0,
    "NAUTILUS_SHELL": 0.0,
    "NETHERRACK": 0.0,
    "NETHER_BRICK": 0.0,
    "NETHER_BRICKS": 0.0,
    "NETHER_BRICK_FENCE": 0.0,
    "NETHER_BRICK_SLAB": 0.0,
    "NETHER_BRICK_STAIRS": 0.0,
    "NETHER_BRICK_WALL": 0.0,
    "NETHER_PORTAL": 0.0,
    "NETHER_QUARTZ_ORE": 0.0,
    "NETHER_STAR": 0.0,
    "NETHER_WART": 0.0,
    "NETHER_WART_BLOCK": 0.0,
    "NOTE_BLOCK": 0.0,
    "OAK_BOAT": 0.0,
    "OAK_BUTTON": 0.0,
    "OAK_DOOR": 0.0,
    "OAK_FENCE": 0.0,
    "OAK_FENCE_GATE": 0.0,
    "OAK_LEAVES": 0.0,
    "OAK_LOG": 0.0,
    "OAK_PLANKS": 0.0,
    "OAK_PRESSURE_PLATE": 0.0,
    "OAK_SAPLING": 0.0,
    "OAK_SIGN": 0.0,
    "OAK_SLAB": 0.0,
    "OAK_STAIRS": 0.0,
    "OAK_TRAPDOOR": 0.0,
    "OAK_WALL_SIGN": 0.0,
    "OAK_WOOD": 0.0,
    "OBSERVER": 0.0,
    "OBSIDIAN": 0.0,
    "OCELOT_SPAWN_EGG": 0.0,
    "ORANGE_BANNER": 0.0,
    "ORANGE_BED": 0.0,
    "ORANGE_CARPET": 0.0,
    "ORANGE_CONCRETE": 0.0,
    "ORANGE_CONCRETE_POWDER": 0.0,
    "ORANGE_DYE": 0.0,
    "ORANGE_GLAZED_TERRACOTTA": 0.0,
    "ORANGE_SHULKER_BOX": 0.0,
    "ORANGE_STAINED_GLASS": 0.0,
    "ORANGE_STAINED_GLASS_PANE": 0.0,
    "ORANGE_TERRACOTTA": 0.0,
    "ORANGE_TULIP": 0.0,
    "ORANGE_WALL_BANNER": 0.0,
    "ORANGE_WOOL": 0.0,
    "OXEYE_DAISY": 0.0,
    "PACKED_ICE": 0.0,
    "PAINTING": 0.0,
    "PANDA_SPAWN_EGG": 0.0,
    "PAPER": 0.0,
    "PARROT_SPAWN_EGG": 0.0,
    "PEONY": 0.0,
    "PETRIFIED_OAK_SLAB": 0.0,
    "PHANTOM_MEMBRANE": 0.0,
    "PHANTOM_SPAWN_EGG": 0.0,
    "PIG_SPAWN_EGG": 0.0,
    "PILLAGER_SPAWN_EGG": 0.0,
    "PINK_BANNER": 0.0,
    "PINK_BED": 0.0,
    "PINK_CARPET": 0.0,
    "PINK_CONCRETE": 0.0,
    "PINK_CONCRETE_POWDER": 0.0,
    "PINK_DYE": 0.0,
    "PINK_GLAZED_TERRACOTTA": 0.0,
    "PINK_SHULKER_BOX": 0.0,
    "PINK_STAINED_GLASS": 0.0,
    "PINK_STAINED_GLASS_PANE": 0.0,
    "PINK_TERRACOTTA": 0.0,
    "PINK_TULIP": 0.0,
    "PINK_WALL_BANNER": 0.0,
    "PINK_WOOL": 0.0,
    "PISTON": 0.0,
    "PISTON_HEAD": 0.0,
    "PLAYER_HEAD": 0.0,
    "PLAYER_WALL_HEAD": 0.0,
    "PODZOL": 0.0,
    "POISONOUS_POTATO": 0.0,
    "POLAR_BEAR_SPAWN_EGG": 0.0,
    "POLISHED_ANDESITE": 0.0,
    "POLISHED_ANDESITE_SLAB": 0.0,
    "POLISHED_ANDESITE_STAIRS": 0.0,
    "POLISHED_DIORITE": 0.0,
    "POLISHED_DIORITE_SLAB": 0.0,
    "POLISHED_DIORITE_STAIRS": 0.0,
    "POLISHED_GRANITE": 0.0,
    "POLISHED_GRANITE_SLAB": 0.0,
    "POLISHED_GRANITE_STAIRS": 0.0,
    "POPPED_CHORUS_FRUIT": 0.0,
    "POPPY": 0.0,
    "PORKCHOP": 0.0,
    "POTATO": 0.0,
    "POTATOES": 0.0,
    "POTION": 0.0,
    "POTTED_ACACIA_SAPLING": 0.0,
    "POTTED_ALLIUM": 0.0,
    "POTTED_AZURE_BLUET": 0.0,
    "POTTED_BAMBOO": 0.0,
    "POTTED_BIRCH_SAPLING": 0.0,
    "POTTED_BLUE_ORCHID": 0.0,
    "POTTED_BROWN_MUSHROOM": 0.0,
    "POTTED_CACTUS": 0.0,
    "POTTED_CORNFLOWER": 0.0,
    "POTTED_DANDELION": 0.0,
    "POTTED_DARK_OAK_SAPLING": 0.0,
    "POTTED_DEAD_BUSH": 0.0,
    "POTTED_FERN": 0.0,
    "POTTED_JUNGLE_SAPLING": 0.0,
    "POTTED_LILY_OF_THE_VALLEY": 0.0,
    "POTTED_OAK_SAPLING": 0.0,
    "POTTED_ORANGE_TULIP": 0.0,
    "POTTED_OXEYE_DAISY": 0.0,
    "POTTED_PINK_TULIP": 0.0,
    "POTTED_POPPY": 0.0,
    "POTTED_RED_MUSHROOM": 0.0,
    "POTTED_RED_TULIP": 0.0,
    "POTTED_SPRUCE_SAPLING": 0.0,
    "POTTED_WHITE_TULIP": 0.0,
    "POTTED_WITHER_ROSE": 0.0,
    "POWERED_RAIL": 0.0,
    "PRISMARINE": 0.0,
    "PRISMARINE_BRICKS": 0.0,
    "PRISMARINE_BRICK_SLAB": 0.0,
    "PRISMARINE_BRICK_STAIRS": 0.0,
    "PRISMARINE_CRYSTALS": 0.0,
    "PRISMARINE_SHARD": 0.0,
    "PRISMARINE_SLAB": 0.0,
    "PRISMARINE_STAIRS": 0.0,
    "PRISMARINE_WALL": 0.0,
    "PUFFERFISH": 0.0,
    "PUFFERFISH_BUCKET": 0.0,
    "PUFFERFISH_SPAWN_EGG": 0.0,
    "PUMPKIN": 0.0,
    "PUMPKIN_PIE": 0.0,
    "PUMPKIN_SEEDS": 0.0,
    "PUMPKIN_STEM": 0.0,
    "PURPLE_BANNER": 0.0,
    "PURPLE_BED": 0.0,
    "PURPLE_CARPET": 0.0,
    "PURPLE_CONCRETE": 0.0,
    "PURPLE_CONCRETE_POWDER": 0.0,
    "PURPLE_DYE": 0.0,
    "PURPLE_GLAZED_TERRACOTTA": 0.0,
    "PURPLE_SHULKER_BOX": 0.0,
    "PURPLE_STAINED_GLASS": 0.0,
    "PURPLE_STAINED_GLASS_PANE": 0.0,
    "PURPLE_TERRACOTTA": 0.0,
    "PURPLE_WALL_BANNER": 0.0,
    "PURPLE_WOOL": 0.0,
    "PURPUR_BLOCK": 0.0,
    "PURPUR_PILLAR": 0.0,
    "PURPUR_SLAB": 0.0,
    "PURPUR_STAIRS": 0.0,
    "QUARTZ": 0.0,
    "QUARTZ_BLOCK": 0.0,
    "QUARTZ_PILLAR": 0.0,
    "QUARTZ_SLAB": 0.0,
    "QUARTZ_STAIRS": 0.0,
    "RABBIT": 0.0,
    "RABBIT_FOOT": 0.0,
    "RABBIT_HIDE": 0.0,
    "RABBIT_SPAWN_EGG": 0.0,
    "RABBIT_STEW": 0.0,
    "RAIL": 0.0,
    "RAVAGER_SPAWN_EGG": 0.0,
    "REDSTONE": 0.0,
    "REDSTONE_BLOCK": 0.0,
    "REDSTONE_LAMP": 0.0,
    "REDSTONE_ORE": 0.0,
    "REDSTONE_TORCH": 0.0,
    "REDSTONE_WALL_TORCH": 0.0,
    "REDSTONE_WIRE": 0.0,
    "RED_BANNER": 0.0,
    "RED_BED": 0.0,
    "RED_CARPET": 0.0,
    "RED_CONCRETE": 0.0,
    "RED_CONCRETE_POWDER": 0.0,
    "RED_DYE": 0.0,
    "RED_GLAZED_TERRACOTTA": 0.0,
    "RED_MUSHROOM": 0.0,
    "RED_MUSHROOM_BLOCK": 0.0,
    "RED_NETHER_BRICKS": 0.0,
    "RED_NETHER_BRICK_SLAB": 0.0,
    "RED_NETHER_BRICK_STAIRS": 0.0,
    "RED_NETHER_BRICK_WALL": 0.0,
    "RED_SAND": 0.0,
    "RED_SANDSTONE": 0.0,
    "RED_SANDSTONE_SLAB": 0.0,
    "RED_SANDSTONE_STAIRS": 0.0,
    "RED_SANDSTONE_WALL": 0.0,
    "RED_SHULKER_BOX": 0.0,
    "RED_STAINED_GLASS": 0.0,
    "RED_STAINED_GLASS_PANE": 0.0,
    "RED_TERRACOTTA": 0.0,
    "RED_TULIP": 0.0,
    "RED_WALL_BANNER": 0.0,
    "RED_WOOL": 0.0,
    "REPEATER": 0.0,
    "REPEATING_COMMAND_BLOCK": 0.0,
    "ROSE_BUSH": 0.0,
    "ROTTEN_FLESH": 0.0,
    "SADDLE": 0.0,
    "SALMON": 0.0,
    "SALMON_BUCKET": 0.0,
    "SALMON_SPAWN_EGG": 0.0,
    "SAND": 0.0,
    "SANDSTONE": 0.0,
    "SANDSTONE_SLAB": 0.0,
    "SANDSTONE_STAIRS": 0.0,
    "SANDSTONE_WALL": 0.0,
    "SCAFFOLDING": 0.0,
    "SCUTE": 0.0,
    "SEAGRASS": 0.0,
    "SEA_LANTERN": 0.0,
    "SEA_PICKLE": 0.0,
    "SHEARS": 0.0,
    "SHEEP_SPAWN_EGG": 0.0,
    "SHIELD": 0.0,
    "SHULKER_BOX": 0.0,
    "SHULKER_SHELL": 0.0,
    "SHULKER_SPAWN_EGG": 0.0,
    "SILVERFISH_SPAWN_EGG": 0.0,
    "SKELETON_HORSE_SPAWN_EGG": 0.0,
    "SKELETON_SKULL": 0.0,
    "SKELETON_SPAWN_EGG": 0.0,
    "SKELETON_WALL_SKULL": 0.0,
    "SKULL_BANNER_PATTERN": 0.0,
    "SLIME_BALL": 0.0,
    "SLIME_BLOCK": 0.0,
    "SLIME_SPAWN_EGG": 0.0,
    "SMITHING_TABLE": 0.0,
    "SMOKER": 0.0,
    "SMOOTH_QUARTZ": 0.0,
    "SMOOTH_QUARTZ_SLAB": 0.0,
    "SMOOTH_QUARTZ_STAIRS": 0.0,
    "SMOOTH_RED_SANDSTONE": 0.0,
    "SMOOTH_RED_SANDSTONE_SLAB": 0.0,
    "SMOOTH_RED_SANDSTONE_STAIRS": 0.0,
    "SMOOTH_SANDSTONE": 0.0,
    "SMOOTH_SANDSTONE_SLAB": 0.0,
    "SMOOTH_SANDSTONE_STAIRS": 0.0,
    "SMOOTH_STONE": 0.0,
    "SMOOTH_STONE_SLAB": 0.0,
    "SNOW": 0.0,
    "SNOWBALL": 0.0,
    "SNOW_BLOCK": 0.0,
    "SOUL_SAND": 0.0,
    "SPECTRAL_ARROW": 0.0,
    "SPIDER_EYE": 0.0,
    "SPIDER_SPAWN_EGG": 0.0,
    "SPLASH_POTION": 0.0,
    "SPONGE": 0.0,
    "SPRUCE_BOAT": 0.0,
    "SPRUCE_BUTTON": 0.0,
    "SPRUCE_DOOR": 0.0,
    "SPRUCE_FENCE": 0.0,
    "SPRUCE_FENCE_GATE": 0.0,
    "SPRUCE_LEAVES": 0.0,
    "SPRUCE_LOG": 0.0,
    "SPRUCE_PLANKS": 0.0,
    "SPRUCE_PRESSURE_PLATE": 0.0,
    "SPRUCE_SAPLING": 0.0,
    "SPRUCE_SIGN": 0.0,
    "SPRUCE_SLAB": 0.0,
    "SPRUCE_STAIRS": 0.0,
    "SPRUCE_TRAPDOOR": 0.0,
    "SPRUCE_WALL_SIGN": 0.0,
    "SPRUCE_WOOD": 0.0,
    "SQUID_SPAWN_EGG": 0.0,
    "STICK": 0.0,
    "STICKY_PISTON": 0.0,
    "STONE": 0.0,
    "STONECUTTER": 0.0,
    "STONE_AXE": 0.0,
    "STONE_BRICKS": 0.0,
    "STONE_BRICK_SLAB": 0.0,
    "STONE_BRICK_STAIRS": 0.0,
    "STONE_BRICK_WALL": 0.0,
    "STONE_BUTTON": 0.0,
    "STONE_HOE": 0.0,
    "STONE_PICKAXE": 0.0,
    "STONE_PRESSURE_PLATE": 0.0,
    "STONE_SHOVEL": 0.0,
    "STONE_SLAB": 0.0,
    "STONE_STAIRS": 0.0,
    "STONE_SWORD": 0.0,
    "STRAY_SPAWN_EGG": 0.0,
    "STRING": 0.0,
    "STRIPPED_ACACIA_LOG": 0.0,
    "STRIPPED_ACACIA_WOOD": 0.0,
    "STRIPPED_BIRCH_LOG": 0.0,
    "STRIPPED_BIRCH_WOOD": 0.0,
    "STRIPPED_DARK_OAK_LOG": 0.0,
    "STRIPPED_DARK_OAK_WOOD": 0.0,
    "STRIPPED_JUNGLE_LOG": 0.0,
    "STRIPPED_JUNGLE_WOOD": 0.0,
    "STRIPPED_OAK_LOG": 0.0,
    "STRIPPED_OAK_WOOD": 0.0,
    "STRIPPED_SPRUCE_LOG": 0.0,
    "STRIPPED_SPRUCE_WOOD": 0.0,
    "STRUCTURE_BLOCK": 0.0,
    "STRUCTURE_VOID": 0.0,
    "SUGAR": 0.0,
    "SUGAR_CANE": 0.0,
    "SUNFLOWER": 0.0,
    "SUSPICIOUS_STEW": 0.0,
    "SWEET_BERRIES": 0.0,
    "SWEET_BERRY_BUSH": 0.0,
    "TALL_GRASS": 0.0,
    "TALL_SEAGRASS": 0.0,
    "TERRACOTTA": 0.0,
    "TIPPED_ARROW": 0.0,
    "TNT": 0.0,
    "TNT_MINECART": 0.0,
    "TORCH": 0.0,
    "TOTEM_OF_UNDYING": 0.0,
    "TRADER_LLAMA_SPAWN_EGG": 0.0,
    "TRAPPED_CHEST": 0.0,
    "TRIDENT": 0.0,
    "TRIPWIRE": 0.0,
    "TRIPWIRE_HOOK": 0.0,
    "TROPICAL_FISH": 0.0,
    "TROPICAL_FISH_BUCKET": 0.0,
    "TROPICAL_FISH_SPAWN_EGG": 0.0,
    "TUBE_CORAL": 0.0,
    "TUBE_CORAL_BLOCK": 0.0,
    "TUBE_CORAL_FAN": 0.0,
    "TUBE_CORAL_WALL_FAN": 0.0,
    "TURTLE_EGG": 0.0,
    "TURTLE_HELMET": 0.0,
    "TURTLE_SPAWN_EGG": 0.0,
    "VEX_SPAWN_EGG": 0.0,
    "VILLAGER_SPAWN_EGG": 0.0,
    "VINDICATOR_SPAWN_EGG": 0.0,
    "VINE": 0.0,
    "VOID_AIR": 0.0,
    "WALL_TORCH": 0.0,
    "WANDERING_TRADER_SPAWN_EGG": 0.0,
    "WATER": 0.0,
    "WATER_BUCKET": 0.0,
    "WET_SPONGE": 0.0,
    "WHEAT": 0.0,
    "WHEAT_SEEDS": 0.0,
    "WHITE_BANNER": 0.0,
    "WHITE_BED": 0.0,
    "WHITE_CARPET": 0.0,
    "WHITE_CONCRETE": 0.0,
    "WHITE_CONCRETE_POWDER": 0.0,
    "WHITE_DYE": 0.0,
    "WHITE_GLAZED_TERRACOTTA": 0.0,
    "WHITE_SHULKER_BOX": 0.0,
    "WHITE_STAINED_GLASS": 0.0,
    "WHITE_STAINED_GLASS_PANE": 0.0,
    "WHITE_TERRACOTTA": 0.0,
    "WHITE_TULIP": 0.0,
    "WHITE_WALL_BANNER": 0.0,
    "WHITE_WOOL": 0.0,
    "WITCH_SPAWN_EGG": 0.0,
    "WITHER_ROSE": 0.0,
    "WITHER_SKELETON_SKULL": 0.0,
    "WITHER_SKELETON_SPAWN_EGG": 0.0,
    "WITHER_SKELETON_WALL_SKULL": 0.0,
    "WOLF_SPAWN_EGG": 0.0,
    "WOODEN_AXE": 0.0,
    "WOODEN_HOE": 0.0,
    "WOODEN_PICKAXE": 0.0,
    "WOODEN_SHOVEL": 0.0,
    "WOODEN_SWORD": 0.0,
    "WRITABLE_BOOK": 0.0,
    "WRITTEN_BOOK": 0.0,
    "YELLOW_BANNER": 0.0,
    "YELLOW_BED": 0.0,
    "YELLOW_CARPET": 0.0,
    "YELLOW_CONCRETE": 0.0,
    "YELLOW_CONCRETE_POWDER": 0.0,
    "YELLOW_DYE": 0.0,
    "YELLOW_GLAZED_TERRACOTTA": 0.0,
    "YELLOW_SHULKER_BOX": 0.0,
    "YELLOW_STAINED_GLASS": 0.0,
    "YELLOW_STAINED_GLASS_PANE": 0.0,
    "YELLOW_TERRACOTTA": 0.0,
    "YELLOW_WALL_BANNER": 0.0,
    "YELLOW_WOOL": 0.0,
    "ZOMBIE_HEAD": 0.0,
    "ZOMBIE_HORSE_SPAWN_EGG": 0.0,
    "ZOMBIE_PIGMAN_SPAWN_EGG": 0.0,
    "ZOMBIE_SPAWN_EGG": 0.0,
    "ZOMBIE_VILLAGER_SPAWN_EGG": 0.0,
    "ZOMBIE_WALL_HEAD": 0.0
  },
  "spawnerValues": {
    "CREEPER": 100000.0,
    "ZOMBIE": 10000.0,
    "SKELETON": 50000.0,
    "DROPPED_ITEM": 0.0,
    "EXPERIENCE_ORB": 0.0,
    "AREA_EFFECT_CLOUD": 0.0,
    "ELDER_GUARDIAN": 0.0,
    "WITHER_SKELETON": 0.0,
    "STRAY": 0.0,
    "EGG": 0.0,
    "LEASH_HITCH": 0.0,
    "PAINTING": 0.0,
    "ARROW": 0.0,
    "SNOWBALL": 0.0,
    "FIREBALL": 0.0,
    "SMALL_FIREBALL": 0.0,
    "ENDER_PEARL": 0.0,
    "ENDER_SIGNAL": 0.0,
    "SPLASH_POTION": 0.0,
    "THROWN_EXP_BOTTLE": 0.0,
    "ITEM_FRAME": 0.0,
    "WITHER_SKULL": 0.0,
    "PRIMED_TNT": 0.0,
    "FALLING_BLOCK": 0.0,
    "FIREWORK": 0.0,
    "HUSK": 0.0,
    "SPECTRAL_ARROW": 0.0,
    "SHULKER_BULLET": 0.0,
    "DRAGON_FIREBALL": 0.0,
    "ZOMBIE_VILLAGER": 0.0,
    "SKELETON_HORSE": 0.0,
    "ZOMBIE_HORSE": 0.0,
    "ARMOR_STAND": 0.0,
    "DONKEY": 0.0,
    "MULE": 0.0,
    "EVOKER_FANGS": 0.0,
    "EVOKER": 0.0,
    "VEX": 0.0,
    "VINDICATOR": 0.0,
    "ILLUSIONER": 0.0,
    "MINECART_COMMAND": 0.0,
    "BOAT": 0.0,
    "MINECART": 0.0,
    "MINECART_CHEST": 0.0,
    "MINECART_FURNACE": 0.0,
    "MINECART_TNT": 0.0,
    "MINECART_HOPPER": 0.0,
    "MINECART_MOB_SPAWNER": 0.0,
    "SPIDER": 0.0,
    "GIANT": 0.0,
    "SLIME": 0.0,
    "GHAST": 0.0,
    "PIG_ZOMBIE": 0.0,
    "ENDERMAN": 0.0,
    "CAVE_SPIDER": 0.0,
    "SILVERFISH": 0.0,
    "BLAZE": 0.0,
    "MAGMA_CUBE": 0.0,
    "ENDER_DRAGON": 0.0,
    "WITHER": 0.0,
    "BAT": 0.0,
    "WITCH": 0.0,
    "ENDERMITE": 0.0,
    "GUARDIAN": 0.0,
    "SHULKER": 0.0,
    "PIG": 0.0,
    "SHEEP": 0.0,
    "COW": 0.0,
    "CHICKEN": 0.0,
    "SQUID": 0.0,
    "WOLF": 0.0,
    "MUSHROOM_COW": 0.0,
    "SNOWMAN": 0.0,
    "OCELOT": 0.0,
    "IRON_GOLEM": 0.0,
    "HORSE": 0.0,
    "RABBIT": 0.0,
    "POLAR_BEAR": 0.0,
    "LLAMA": 0.0,
    "LLAMA_SPIT": 0.0,
    "PARROT": 0.0,
    "VILLAGER": 0.0,
    "ENDER_CRYSTAL": 0.0,
    "TURTLE": 0.0,
    "PHANTOM": 0.0,
    "TRIDENT": 0.0,
    "COD": 0.0,
    "SALMON": 0.0,
    "PUFFERFISH": 0.0,
    "TROPICAL_FISH": 0.0,
    "DROWNED": 0.0,
    "DOLPHIN": 0.0,
    "CAT": 0.0,
    "PANDA": 0.0,
    "PILLAGER": 0.0,
    "RAVAGER": 0.0,
    "TRADER_LLAMA": 0.0,
    "WANDERING_TRADER": 0.0,
    "FOX": 0.0,
    "BEE": 0.0,
    "FISHING_HOOK": 0.0,
    "LIGHTNING": 0.0,
    "PLAYER": 0.0,
    "UNKNOWN": 0.0
  }
}
```
<h2>quests.json</h2>

```json
{
  "islandQuestGUITitle": "&bIsland Quests",
  "islandQuestGUIBackgroundItem": {
    "material": "BLACK_STAINED_GLASS_PANE",
    "name": "&9",
    "lore": [],
    "amt": 1
  },
  "islandQuestGUIRows": 3,
  "questOrder": [
    "Quest-1",
    "Quest-2",
    "Quest-3",
    "Quest-4",
    "Quest-5",
    "Quest-6",
    "Quest-7",
    "Quest-8",
    "Quest-9",
    "Quest-10",
    "Quest-11",
    "Quest-12",
    "Quest-13",
    "Quest-14",
    "Quest-15",
    "Quest-16",
    "Quest-17",
    "Quest-18",
    "Quest-19"
  ],
  "useQuestOrder": true,
  "sendNextQuestInOrderMessages": true,
  "islandQuests": [
    {
      "id": "Quest-1",
      "name": "Get wood from your island's tree",
      "guiDisplayItem": {
        "material": "OAK_WOOD",
        "name": "&bGet wood from island's tree",
        "lore": [
          "&7Break the wood from your island's tree trunk",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 0,
      "type": "BREAK_BLOCKS",
      "goalParameter": "OAK_LOG",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)",
          "command(give {player} oak_sapling 1:::give {player} apple 1)"
        ]
      }
    },
    {
      "id": "Quest-2",
      "name": "Craft a wooden pickaxe",
      "guiDisplayItem": {
        "material": "WOODEN_PICKAXE",
        "name": "&bCraft a Wooden Pickaxe",
        "lore": [
          "&7Put three planks and 2 sticks in a crafting table.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 1,
      "type": "CRAFT",
      "goalParameter": "WOODEN_PICKAXE",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress 0/0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-3",
      "name": "Make a ore generator",
      "guiDisplayItem": {
        "material": "LAVA_BUCKET",
        "name": "&8Create an Ore Generator",
        "lore": [
          "&7Mine &b3 &7cobblestone from Ore Generator",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 2,
      "type": "BREAK_BLOCKS",
      "goalParameter": "COBBLESTONE",
      "amountTillComplete": 2,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-4",
      "name": "Craft a Stone Pickaxe",
      "guiDisplayItem": {
        "material": "STONE_PICKAXE",
        "name": "&8Craft a stone pickaxe.",
        "lore": [
          "&7Craft a Stone Pickaxe",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 3,
      "type": "CRAFT",
      "goalParameter": "STONE_PICKAXE",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-5",
      "name": "Mine 3 Iron Ore",
      "guiDisplayItem": {
        "material": "IRON_ORE",
        "name": "&8Mine 3 Iron Ore from the Ore Generator.",
        "lore": [
          "&7Mine &b3 Iron Ore.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 4,
      "type": "BREAK_BLOCKS",
      "goalParameter": "IRON_ORE",
      "amountTillComplete": 3,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-6",
      "name": "Craft an Furnace",
      "guiDisplayItem": {
        "material": "FURNACE",
        "name": "&8Craft a Furnace",
        "lore": [
          "&7Place 8 cobblestone blocks in the crafting table.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 5,
      "type": "CRAFT",
      "goalParameter": "FURNACE",
      "amountTillComplete": 8,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)",
          "command(give {player} coal 1)"
        ]
      }
    },
    {
      "id": "Quest-7",
      "name": "Smelt Iron Ingot",
      "guiDisplayItem": {
        "material": "IRON_INGOT",
        "name": "&8Smelt Iron Ingot",
        "lore": [
          "&7Smelt 3 Iron Ingots in a furnace.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 6,
      "type": "SMELT",
      "goalParameter": "IRON_INGOT",
      "amountTillComplete": 3,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-8",
      "name": "Craft an &bIron Pickaxe",
      "guiDisplayItem": {
        "material": "IRON_PICKAXE",
        "name": "&8Craft an Iron Pickaxe",
        "lore": [
          "&7Place three Iron Ingots and 2 Sticks into a crafting table.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 7,
      "type": "CRAFT",
      "goalParameter": "IRON_PICKAXE",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-9",
      "name": "Plant a Sapling",
      "guiDisplayItem": {
        "material": "OAK_SAPLING",
        "name": "&8Plant a sapling.",
        "lore": [
          "&7Plant the Oak Sapling in your Inventory.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 8,
      "type": "PLACE_BLOCKS",
      "goalParameter": "OAK_SAPLING",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-10",
      "name": "&8Get some sand.",
      "guiDisplayItem": {
        "material": "SAND",
        "name": "&8Get some sand.",
        "lore": [
          "&7Dig into your island and find the sand.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 9,
      "type": "BREAK_BLOCKS",
      "goalParameter": "SAND",
      "amountTillComplete": 3,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-11",
      "name": "&8Plant some Cactus.",
      "guiDisplayItem": {
        "material": "CACTUS",
        "name": "&8Plant some cactus.",
        "lore": [
          "&7Plant some cactus on sand.",
          "&7You can find cactus in the island chest",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 10,
      "type": "PLACE_BLOCKS",
      "goalParameter": "CACTUS",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-12",
      "name": "&8Plant some sugarcane.",
      "guiDisplayItem": {
        "material": "SUGAR_CANE",
        "name": "&8Plant some sugarcane.",
        "lore": [
          "&7Plant some sugarcane on sand.",
          "&7You can find some sugarcane in the island chest.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 11,
      "type": "PLACE_BLOCKS",
      "goalParameter": "CACTUS",
      "amountTillComplete": 10,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-13",
      "name": "&8Plant some melons.",
      "guiDisplayItem": {
        "material": "MELON_SLICE",
        "name": "&8Plant some melons.",
        "lore": [
          "&7Plant some melons on tilled dirt.",
          "&7You can find some melon seeds in the island chest.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 12,
      "type": "PLACE_BLOCKS",
      "goalParameter": "MELON_SEEDS",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-14",
      "name": "&8Plant 20 Cacti.",
      "guiDisplayItem": {
        "material": "CACTUS",
        "name": "&8Make a cactus farm.",
        "lore": [
          "&7Plant 20 cacti.",
          "&7You can buy more sand from /is shop.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 13,
      "type": "PLACE_BLOCKS",
      "goalParameter": "CACTUS",
      "amountTillComplete": 20,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-15",
      "name": "&8Plant 30 wheat seeds.",
      "guiDisplayItem": {
        "material": "WHEAT_SEEDS",
        "name": "&8Make a wheat farm.",
        "lore": [
          "&7Plant some wheat on dirt.",
          "&7You can buy more dirt from /is shop.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 14,
      "type": "PLACE_BLOCKS",
      "goalParameter": "WHEAT_SEEDS",
      "amountTillComplete": 30,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-16",
      "name": "&8Harvest some wheat.",
      "guiDisplayItem": {
        "material": "WHEAT",
        "name": "&8Harvest some wheat.",
        "lore": [
          "&7Harvest some fully grown wheat.",
          "&7You can find some pumpkin in the island chest.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 15,
      "type": "BREAK_BLOCKS",
      "goalParameter": "WHEAT",
      "amountTillComplete": 1,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-17",
      "name": "&8Kill 100 Zombies.",
      "guiDisplayItem": {
        "material": "ZOMBIE_HEAD",
        "name": "&8Kill Zombies.",
        "lore": [
          "&7Kill 100 Zombies.",
          "&7They will spawn in the dark.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 16,
      "type": "KILL_MOBS",
      "goalParameter": "ZOMBIE",
      "amountTillComplete": 100,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-18",
      "name": "&8Kill 100 Skeleton.",
      "guiDisplayItem": {
        "material": "SKELETON_SKULL",
        "name": "&8Kill Skeletons.",
        "lore": [
          "&7Kill 100 Skeletons.",
          "&7They will spawn in the dark.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 17,
      "type": "KILL_MOBS",
      "goalParameter": "SKELETON",
      "amountTillComplete": 100,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    },
    {
      "id": "Quest-19",
      "name": "&8Kill 100 Creepers.",
      "guiDisplayItem": {
        "material": "CREEPER_HEAD",
        "name": "&8Kill Creepers.",
        "lore": [
          "&7Kill 100 Creepers.",
          "&7They will spawn in the dark.",
          "&7Completion: &b{currentAmount}&7/&b{finalAmount}"
        ],
        "amt": 1
      },
      "guiDisplayIndex": 16,
      "type": "KILL_MOBS",
      "goalParameter": "CREEPER",
      "amountTillComplete": 100,
      "oneTime": true,
      "actionsOnActivation": {
        "actions": [
          "message(&7You have started the {quest-name}:::&7Your current progress is 0/{quest-amount-till-complete})",
          "actionbar(&7Your quest progress is 0/{quest-amount-till-complete})"
        ]
      },
      "actionsOnCompletion": {
        "actions": [
          "message(&7You have finished the {quest-name}:::&7Your current progress is {quest-amount-till-complete}/{quest-amount-till-complete})",
          "title(&7{quest-name}:::&b&lQuest Completed)"
        ]
      }
    }
  ]
}
```
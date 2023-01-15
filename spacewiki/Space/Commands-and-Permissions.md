# 指令

| 指令 | 说明 | 权限 |
| --- | --- | --- |
| `/space` | 打开Space的Gui | None |
| `/space admin` | 打开Space管理员页面 | `space.admin` |
| `/space advancement (grant\|revoke) <player> <advancement>` | 给予或撤销玩家的进度.<br>请确保你装了 [Crazy Advancements API](https://www.spigotmc.org/resources/crazy-advancements-api.51741/)插件. | `space.advancement` |
| `/space astronauts` | 打开一个Gui，列出所有在星球上的玩家 | `space.view` |
| `/space backup` | 备份Space配置文件 | `space.backup` |
| `/space charge [(all) (set)] [charge]` | 为玩家手中的物品或所有在玩家背包中的物品充满电 | `space.charge` |
| `/space cheat` | 打开作弊界面. | `space.cheat` |
| `/space give <player> <item> (<count>)` | 给予一个玩家Space物品. 当然你可以使用 "*" 来代指所有在线的玩家 | `space.give` |
| `/space guide` | 给予玩家一个太空指南. | `space.guide` |
| `/space wiki` | 显示Wiki界面. | `space.wiki` |
| `/space hooks` | 列出当前与Space接口链接的插件以及版本 | `space.hooks` |
| `/space unstuck` | 如果你因重力或某种原因被卡在障碍物中，可以使用指令来防卡 | `space.unstuck` |
| `/space module <grant/revoke/toggle> <module>` | Adds/removes/toggles modules on the handheld armor part | `space.module` |
| `/space reload` | Reloads the Space configuration files. | `space.reload` |
| `/space station` | On first use, purchases a Space Station.<br>On every subsequent use, teleports the player to their Space Station. | `space.station.create` |
| `/space station reset <player>` | Resets your Space Station, or that of another player. | `space.station.reset`, `space.station.reset.other` |
| `/space station tp <player>` | Teleports the player to another player's Space Station. | `space.station.teleport` |
| `/space summon <entity> [(-baby)]` | Summons a Space entity. | `space.summon` |
| `/space version` | Displays the current version of Space. | `space.version` |
| `/space enchant <enchantment>` | Applies the enchantment to the handheld item | `space.enchant` |
| `/space schematic <schematic>` | Summons the schematic at your position | `space.schematic` |
| `/space gui <gui>` | Opens the relevant GUI | `space.gui.fabricator`, `space.gui.modularworkbench`, `space.gui.printer`, `space.gui.quantumworkbench`, `space.gui.trashcan`, `space.gui.rocket`, `space.gui.atomiser` |

# Permissions

| Permission | Description |
| --- | --- |
| `space.admin` | **(DEPRECATED; Use `space.*` instead)** Permits everything, including `/space admin`. |
| `space.advancement` | Permits usage of `/space advancement (grant\|revoke) <player> <module>` (if [Crazy Advancements API](https://www.spigotmc.org/resources/crazy-advancements-api.51741/) is installed). |
| `space.backup` | Permits usage of `/space backup`. |
| `space.charge` | Permits usage of `/space charge [(all) (set)] [charge]`. |
| `space.commandsigns.create` | Permits creation of [Command Signs](Command-Signs). |
| `space.commandsigns.use` | Permits usage of Command Signs. |
| `space.debug` | Permits usage of [Debug Wands](Debug-Wand). |
| `space.give` | Permits usage of `/space give <player> <item> (<count>)`. |
| `space.guide` | Permits usage of `/space guide`. |
| `space.schematic` | Permits usage of `/space schematic`. |
| `space.wiki` | Permits usage of `/space wiki`. |
| `space.hooks` | Permits usage of `/space hooks`. |
| `space.unstuck` | Permits usage of `/space unstuck`. |
| `space.module` | Permits usage of `/space module`. |
| `space.regionbypass` | Bypasses region protection in [GriefPrevention](https://www.spigotmc.org/resources/griefprevention.1884/), [Lands](https://www.spigotmc.org/resources/lands-land-claim-plugin-grief-prevention-protection-gui-management-nations-wars-1-16-support.53313/), and [Towny](https://www.spigotmc.org/resources/towny-advanced.72694/). |
| `space.reload` | Permits usage of `/space reload`. |
| `space.enchant` | Permits usage of `/space enchant`. |
| `space.station.create` | Permits usage of `/space station`. |
| `space.station.reset`, `space.station.reset.other` | Permits usage of `/station reset <player>`. |
| `space.station.teleport` | Permits usage of `/station tp <player>`. |
| `space.summon` | Permits usage of `/space summon <entity> [(-baby)]`. |
| `space.update` | Enables a notification for whether the plugin is outdated, displayed upon joining. |
| `space.version` | Permits usage of `/space version`. |
| `space.view` | Permits usage of `/space astronauts`. |
| `space.gui.fabricator` | Permits usage of `/space gui fabricator`. |
| `space.gui.modularworkbench` | Permits usage of `/space gui modularworkbench`. |
| `space.gui.printer` | Permits usage of `/space gui printer`. |
| `space.gui.quantumworkbench` | Permits usage of `/space gui modularworkbench`. |
| `space.gui.trashcan` | Permits usage of `/space gui trashcan`. |
| `space.gui.rocket` | Permits usage of `/space gui rocket`. |
| `space.gui.atomiser` | Permits usage of `/space gui atomiser`. |
| `space.immunity.oxygen` | Allows the player to be immune to oxygen damage effects. Only valid if `Immunity-Permissions-Enabled` is set to `true` |
| `space.immunity.temperature.*` | Allows the player to be immune to all temperature damage effects. Only valid if `Immunity-Permissions-Enabled` is set to `true` |
| `space.immunity.temperature.hot` | Allows the player to be immune to hot environment damage effects. Only valid if `Immunity-Permissions-Enabled` is set to `true` |
| `space.immunity.temperature.cold` | Allows the player to be immune to cold environment damage effects. Only valid if `Immunity-Permissions-Enabled` is set to `true` |
| `space.immunity.acidrain` | Allows the player to be immune to acid rain damage effects. Only valid if `Immunity-Permissions-Enabled` is set to `true` |
| `space.immunity.radiation` | Allows the player to be immune to radiation damage effects. Only valid if `Immunity-Permissions-Enabled` is set to `true` |
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
| `/space module <grant/revoke/toggle> <module>` | 在你手持的装备上添加/删除/切换模块 | `space.module` |
| `/space reload` | 重新加载Space配置文件 | `space.reload` |
| `/space station` | 第一次使用时将会提示您购买一个空间站<br>当购买完后再使用这个指令会传送到空间站 | `space.station.create` |
| `/space station reset <player>` | 重置一个玩家的空间站 | `space.station.reset`, `space.station.reset.other` |
| `/space station tp <player>` | 传送到一个玩家的空间站 | `space.station.teleport` |
| `/space summon <entity> [(-baby)]` | 召唤一个Space生物 | `space.summon` |
| `/space version` | 显示当前的Space版本 | `space.version` |
| `/space enchant <enchantment>` | 为你的手持物品添加一个附魔 | `space.enchant` |
| `/space schematic <schematic>` | 在你当前的位置生成一个Space建筑 | `space.schematic` |
| `/space gui <gui>` | 打开相关的Gui | `space.gui.fabricator`, `space.gui.modularworkbench`, `space.gui.printer`, `space.gui.quantumworkbench`, `space.gui.trashcan`, `space.gui.rocket`, `space.gui.atomiser` |

# 权限

| Permission | Description |
| --- | --- |
| `space.admin` | **(已经弃用; 请使用 `space.*` 来代替)** 允许使用任何指令, 包括 `/space admin`. |
| `space.advancement` | 允许使用指令 `/space advancement (grant\|revoke) <player> <module>` (如果你安装了 [Crazy Advancements API](https://www.spigotmc.org/resources/crazy-advancements-api.51741/) 插件). |
| `space.backup` | 允许使用指令： `/space backup`. |
| `space.charge` | 允许使用指令： `/space charge [(all) (set)] [charge]`. |
| `space.commandsigns.create` | 允许使用指令： [告示牌命令](/Space/Command-Signs). |
| `space.commandsigns.use` | 允许使用告示牌指令. |
| `space.debug` | Permits usage of [Debug Wands](/Space/Debug-Wand). |
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
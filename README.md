# MCFFA
## Overview

This plugin can help you start FFA faster.
This plug-in is maintained by only one person and the update speed is very slow. Please forgive me.

## Commands

- `/ffa join <Map>` - Enter the designated map and be randomly teleported (with security protection)
- `/ffa reload` - Reload Config File
- `/ffa spawn` - Eleport to the specified respawn point
- `/ffa setspawn` - Set your respawn point

## Function

- Database support (Kill and Died will record in database)
- Customized spawn point
- Customize Give Armor
- multiple languages (Simplified Chinese, Traditional Chinese, Spanish, Japanese)

## Configuration

The configuration file (`config.yml`) includes the following options:

```yaml
# Random Teleport Setting
Teleport_Max: 1000
Safe_Count: 10
Limit_Time: 5

# Language
Language: "zh_TW.yml"

# Attention: Please use the correct format
# For example: diamond_sword:1
# discord_sword is item, 1 is amount
# If you use the wrong format, nothing will happen
Status_Armor: false # false or true
Armor:
  - diamond_sword:1
  - diamond_helmet:1
  - diamond_chestplate:1
  - diamond_leggings:1
  - diamond_boots:1
  - golden_apple:10


# Teleport to Spawn | (Second)
Status_Countdown: false # false or true
Countdown: 3

# DataBase, For example : jdbc:mysql://localhost:3306/<name>
Status_DataBase: false # false or true
URL: "null"
UserName: "root"
password: "null"

# Ranking Recode Setting
# If a player is killed by another player on the map you specify,
# the number of deaths and kills will be recorded in the database.
# Can be more than one
Status_Ranking_Recode: false # false or true
World:
  - World1
  - World2
  - World3

# Settings for rebirth when the player dies
# For example if you died or use command /spawn, you will teleport to world X Y Z
Status_Respawn: false # false or true
Respawn_World: world
Respawn_X: 0
Respawn_Y: 86
Respawn_Z: 0
```
### 
 © CopyRight 2024 Snowball

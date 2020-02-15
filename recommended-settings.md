<p align="center">
  <img src="113.png" alt="Jagged Alliance 2 1.13">
</p>

# Jagged Alliance 2 v1.13 - Recommended Settings

> **THIS DOCUMENT IS A WORK IN PROGRESS.**

> This documentation is up to date as of 1.13 r8741.

This document contains some settings the authors of this document recommend looking at to potentially make the game more enjoyable.

## 1. INI tweaks
The following settings can be found in `\Data-1.13\JA2_Options.ini`.

> The `1.13` part should be replaced if playing a mod other than 1.13, e.g. `\Data-AIM\JA2_Options.ini` for AIMNAS.

> **Do not use the included INI editor. It is known to cause problems.** To edit INI and XML files, use a text editor such as as [Notepad++](https://notepad-plus-plus.org/).

|  r7609  |  r8741  | Setting | Description |
|  :---:  |  :---:  |   ---   |     ---     |
| &check; | &check; | `TRIGGER_MASSIVE_ENEMY_COUNTERATTACK_AT_DRASSEN` | Should be set to `FALSE` for a new player. It is infamous for being very difficult to handle so early in the campaign. |
| &cross; | &check; | `REDUCED_INSTANT_DEATH` | Lowers lethal damage to cause the merc to fall into a coma rather than die. Makes merc deaths less likely. |
| &check; | &check; | `MINE_INCOME_PERCENTAGE` | Changes how much cash mines generate. |
| &check; | &check; | `WHICH_MINE_SHUTS_DOWN` | Controls which mine will run out of ore and stop working. |
| &check; | &check; | `STEALING_FROM_SHIPMENTS_DISABLED` | Disables stealing from shipments (e.g. Pablo in Drassen). |
| &check; | &check; | `CHANCE_OF_SHIPMENT_LOSS` | Sets the chance of a whole shipment from Bobby Ray being lost. |
| &check; | &check; | `CHANCE_TONY_AVAILABLE` | Can be set to 100% if you always want to meet Tony (a useful fellow). |
| &check; | &check; | `ENABLE_ALL_WEAPON_CACHES` | Enables all sectors with "secret" weapon caches. |
| ~ | &check; | `DROP_ALL` | Normally, enemies have a chance to drop items when killed. `1` forces all items to drop. `2`  will also drop all but the items that wouldn't have dropped normally are severely damaged. In r7609, this setting is available on the New Game screen. |
| &check; | &check; | `SELL_ITEMS_WITH_ALT_LMB` | Allows the player to sell their items directly from the sector inventory screen whenever they wish. |
| &check; | ~ | `ALLOW_REINFORCEMENTS` | Allows enemies/militia to reinforce an adjacent sector. They arrive at the edge of the map a few turns after the battle starts. As of r8741, this setting is in `TableData\DifficultySettings.xml` (see XML tweaks section of this page). |
| &check; | &check; | `MERCS_CAN_BE_ON_ASSIGNMENT` | Decides if all mercs will be available at the start of the game and if they will go on other assignments during the campaign. |
| &check; | &check; | `MERCS_CAN_DIE_ON_ASSIGNMENT` | Allows mercs to die when away on other assignments. |
| &check; | &check; | `SHOW_SKILLS_IN_HIRING_PAGE` | Shows skills and traits as a tooltip on a merc's portrait in both the AIM & MERC hiring page. |
| &check; | &check; | `SLAY_STAYS_FOREVER` | Determines if a character, Slay, will stay with your team indefinitely. |


## 2. XML tweaks
All XML files can be found in in the `\Data-1.13\TableData` directory.
> The `1.13` part should be replaced if playing a mod other than 1.13, e.g. `\Data-AIM\TableData` for AIMNAS.

> Older versions of 1.13 included a tool for this, `XMLEditor`, but it was removed because it caused problems.

### 2.1 Starting money
To change the amount of money you start with, open `\Data-1.13\TableData\DifficultySettings.xml` and edit the `<StartingCash>` value of the difficulty you want to play.

### 2.2 Vehicle capacity
By default, the helicopter, hummer and ice cream truck all hold a maximum of six mercs. If you are fielding larger squads than this, you can edit each vehicle's capacity to make squad movement easier.

In `\Data-1.13\TableData\Vehicles.xml`, find `<uiIndex>` 160 (hummer), 162 (ice cream truck) and 163 (helicopter). For each, you can change the `<SeatingCapacities>` value from 6 to 8, 10, or whatever you want.

> Warning: the game may crash if your squad size is smaller than the vehicle capacity and you enter combat while in a vehicle.

### 2.3 Reinforcements
This feature allows enemies/militia to reinforce an adjacent sector. They arrive at the edge of the map a few turns after the battle starts. To disable this, open `\Data-1.13\TableData\DifficultySettings.xml` and set the `<AllowReinforcements>` value to `0` for the difficulty you want to play.

> In r7609 this is controlled by `ALLOW_REINFORCEMENTS` in `JA2_Options.ini`. See the above INI tweaks section for more info.


## 3. Advanced
<!-- TODO: move this section to another page titled "advanced settings/configuration" -->
The authors of this document take no responsibility for any unintended behaviour caused by the following, third-party software.

### 3.1 dgVoodoo 2
TODO  
https://www.pcgamingwiki.com/wiki/DgVoodoo_2

### 3.2 IntegerScaler
TODO  
https://tanalin.com/en/projects/integer-scaler/

### 3.3 Wine
TODO  
https://www.winehq.org/
# Recommended Settings
## 0 Intro
Listed below are some settings we recommend taking a look at to potentially make the game more enjoyable for you.

Note regarding directories: wherever you see `\Data-1.13\...`, the `1.13` part should be replaced if playing a mod other than 1.13, e.g. `\Data-AIM\...` for AIMNAS.


## 1 INI tweaks
The following settings can be found in `\Data-1.13\JA2_Options.ini`.

### 1.1 Difficulty related
- `TRIGGER_MASSIVE_ENEMY_COUNTERATTACK_AT_DRASSEN` should be set to `FALSE` for a new player. It is somewhat infamous for being very difficult to handle so early in the campaign.
- `SELL_ITEMS_WITH_ALT_LMB` allows the player to sell their items from the sector inventory screen whenever they wish.
- `MINE_INCOME_PERCENTAGE` changes how much cash mines generate. Can be used to make the game easier or harder.
- `STEALING_FROM_SHIPMENTS_DISABLED` can disable stealing from shipments (e.g. Pablo in Drassen).
- `CHANCE_OF_SHIPMENT_LOSS` sets the chance of a whole shipment from Bobby Ray being lost.
- `CHANCE_TONY_AVAILABLE` can be set to 100% if you always want to meet Tony (a useful fellow).

### 1.2 Misc. settings
- `MERCS_CAN_BE_ON_ASSIGNMENT` changes if all mercs will be available at the start of the game and if they will go on other assignments during the campaign.
- `MERCS_CAN_DIE_ON_ASSIGNMENT` allows mercs to die when away on other assignments.
- `SHOW_SKILLS_IN_HIRING_PAGE` shows skills and traits as a tooltip on a merc's portrait in both the AIM & MERC hiring page.


## 2 XML tweaks
All XML files can be found in in the `\Data-1.13\TableData` directory.

### 2.1 Starting money
To change the amount of money you start with, open `\Data-1.13\TableData\DifficultySettings.xml` and edit the `<StartingCash>` value of the difficulty you want to play.

### 2.2 Vehicle capacity
By default, the helicopter, hummer and ice cream truck all hold a maximum of six mercs. If you are fielding larger squads than this, you can edit each vehicle's capacity to make squad movement easier.

In `\Data-1.13\TableData\Vehicles.xml`, find `<uiIndex>` 160 (hummer), 162 (ice cream truck) and 163 (helicopter). For each, you can change the `<SeatingCapacities>` value from 6 to 8, 10, or whatever you want.

# 0 Intro

## 0.1 Preamble

**WORK IN PROGRESS**

This document is an attempt to create clear and structured starter documentation for people who want to start playing 1.13.  
From years of hanging around in the [Bear's Pit community](http://thepit.ja-galaxy-forum.com/) we noticed there's a complete lack of explanation how to get started with this mod and everything surrounding it.

This documentation is up to date as of version XXXX.

## 0.2 What is 1.13?

Jagged Alliance 2 v1.13 is a MODIFICATION for the Jagged Alliance 2 game, with a host of new features and improvements, as well as externalizing a lot of data to make modding easier.  
Lots of features have been added like new resolutions, improved AI, weather effects and new items. 1.13 does still contain the original maps and quests.
The 1.13 mod has been structured in such a way that it can be used as a baseline for creating new mods.

## 0.3 List of Features
TODO


# 1 Installation

To install 1.13 you will have to go through a few steps.

## 1.1 Jagged Alliance 2

To be able to play 1.13 you will need to own the Jagged Alliance 2 game itself, there are several places where you can still get the game, for example:  

- GOG https://www.gog.com/game/jagged_alliance_2
- Steam https://store.steampowered.com/app/1620/Jagged_Alliance_2_Gold/

After you got your hand on a copy of JA2 and want to go install it, we have a few tips for you to make sure everything runs smooth.

- Don't install the game to a default folder like `C:\Program Files` or `C:\Program Files (x86)`, instead make a folder like `C:\Games` (depending on your disk setup) and install the game there.
- After installing Jagged Alliance, make a backup of the folder so you dont have to do a reinstallation each time you want to start from scratch, so for example copy the `Jagged Alliance 2` folder in `C:\Games` to a backup copy, technically you can make endless copies of the JA2 folder for different 1.13 mod based installations, the naming of the folder doesn't really matter to be able to play 1.13.
- If you wonder how you will be able to use the Steam version of JA2, you can find it in the installation directory of Steam, usually in a place like `C:\Program Files\Steam\steamapps\` you can make a copy of the Jagged Alliance 2 folder from there to a place like `C:\Games`

## 1.2 The 1.13 mod

Once you have your clean JA2 installation ready to be turned into a clean 1.13 installation, there are a few routes you can go to achieve this.

- Install the latest SCI (Single Click Installer, something of a misnomer). This is the best way to go as these SCI packages are based upon the latest game developments but don't worry, they are very stable.
- Install the old so called "stable" release which is referred to as 7609. Some mods chose to stick to this version so check what your goal mod requires.
- Install 1.13 via the SVN route. This is an expert path because next to getting all the mod files from SVN you will have to compile the game's executable file from source code as well.

### 1.2.1 Install the latest SCI 

This is the preferred way to go for people who want to start playing 1.13, it will give you a good out of the box experience.  
You can get the latest SCI file from the following OneDrive location [link](https://onedrive.live.com/?id=13A6926EAC52083!583&cid=013A6926EAC52083)  
If you sort the OneDrive file listing from new to old you should see the file with the highest revision number up on top, download this one.  

Once you have downloaded the file you will need to extract it, there are different tools to use for this like [7-Zip](https://www.7-zip.org/ "7-Zip homepage")  
Extract the file to the location where your target JA2 installation is located and choose to overwrite files if you get asked, so for this example we'll use "C:\Games\Jagged Alliance 2\"  

### 1.2.2 Install release 7609

For the special cases with a requirement to run on release 7609, you can find it on the [official 1.13 wiki site](http://ja2v113.pbworks.com/w/page/4218334/Downloads)

TODO

### 1.2.3 Install 1.13 from SVN

If you have a special reason to not use the SCI release, for example if you are actively helping to fix bugs in 1.13, it can be handy to get your gamedata and executable from source, this is however an advanced topic.


## 1.3 Fixes for newer Windows versions
TODO

### 1.3.1 Windows 8+
TODO

There are a few things you will need to do to be able to play 1.13 well on the Windows 8+ versions, here's a list:

- Wine DLLs
- registry fix for 16-bit color mode
- running on one CPU thread

The Wine DLLs and registry fix can be found at `\Docs\Windows Compatibility Fixes\Windows 7-10 Fix.zip`. Make sure to read the included readme!

To run the game on a single CPU thread, check out [these instructions](https://www.eightforums.com/threads/processor-affinity-set-for-applications-in-windows-8.24086/).

### 1.3.2 Windows 7 and older

Technically, there is no need to adjust anything to make 1.13 run well on Windows 7 and older.


# 2 Playing 1.13
TODO

## 2.1 Starting a new game
TODO

## 2.2 Game settings
TODO

### 2.2.1 New Game Settings
TODO: descriptions and lists of possible values
TODO: list 7609 options
The following is from build 8657:
- Difficulty level [Novice, Experienced, Expert, Insane]
- Skill Traits
- Game Style
- Extra Difficulty
- Inventory / Attachments
- Progress Speed of Item Choices
- Available Arsenal
- Max. Squad Size
- Bobby Ray Quality
- Bobby Ray Quantity
Missing setting? -> refer to section 2.3.1

### 2.2.2 Config files
TODO
Part of the beauty of the 1.13 mod is just how much control the player has to tailor the experience to their own tastes. This is done via a number of config files.
**Do not use the included INI editor. It is known to cause problems.** To edit INI and XML files, use a text editor. Preferably, one that is more sophisticated than Windows's Notepad, such as [Notepad++](https://notepad-plus-plus.org/).
#### 2.2.2.1 ja2.ini
TODO
Found in the root directory (i.e. aside `ja2.exe`). Manages global settings such as resolution and enabling windowed mode.
#### 2.2.2.2 JA2_Options.ini
TODO
Found in the `Data-1.13` directory. This is where you will find the bulk of the settings for 1.13.
TODO: list some commonly used / useful settings to change 
#### 2.2.2.3 XML Files
TODO
Found in the `\Data-1.13\TableData` directory.

## 2.3 Frequently Asked Settings

### 2.3.1 Disappeared New Game Settings
TODO
In build XXXX, some of the New Game settings were moved to `JA2_Options.ini`.

### 2.3.2 Starting Cash
To change the amount of money you start with, open `\Data-1.13\TableData\DifficultySettings.xml` and edit the `<StartingCash>` value of the difficulty you want to play.

### 2.3.3 NCTH/OCTH
TODO

### 2.3.4 Drassen counterattack is too difficult!
JA2_Options.ini: Set `TRIGGER_MASSIVE_ENEMY_COUNTERATTACK_AT_DRASSEN` to `FALSE`.

## 2.4 More settings of interest

### 2.4.1 INI tweaks
The following settings can be found in `JA2_Options.ini`.

#### 2.4.1.1 Difficulty related
- `SELL_ITEMS_WITH_ALT_LMB` allows the player to sell their items from the sector inventory screen whenever they wish.
- `MINE_INCOME_PERCENTAGE` changes how much cash mines generate. Can be used to make the game easier or harder.
- `STEALING_FROM_SHIPMENTS_DISABLED` can disable stealing from shipments (e.g. Pablo in Drassen).
- `CHANCE_OF_SHIPMENT_LOSS` sets the chance of a whole shipment from Bobby Ray being lost.
- `CHANCE_TONY_AVAILABLE` can be set to 100% if you always want to meet Tony (a useful fellow).

#### 2.4.1.2 Misc. settings
- `MERCS_CAN_BE_ON_ASSIGNMENT` changes if all mercs will be available at the start of the game and if they will go on other assignments during the campaign.
- `MERCS_CAN_DIE_ON_ASSIGNMENT` allows mercs to die when away on other assignments.
- `SHOW_SKILLS_IN_HIRING_PAGE` shows skills and traits as a tooltip on a merc's portrait in both the AIM & MERC hiring page.

### 2.4.2 XML tweaks

#### 2.4.2.1 Vehicle capacity
By default, the helicopter, hummer and ice cream truck all hold a maximum of six mercs. If you are fielding larger squads than this, you can edit each vehicle's capacity to make squad movement easier.

In `\Data-1.13\TableData\Vehicles.xml`, find `<uiIndex>` 160 (hummer), 162 (ice cream truck) and 163 (helicopter). For each, you can change the `<SeatingCapacities>` value from 6 to 8, 10, or whatever you want.


# 3 Mods
TODO

## 3.1 AIMNAS
TODO

## 3.2 Urban Chaos 1.13
TODO

## 3.3 Vengeance 1.13 Reloaded
TODO

## 3.4 Arulco Revisited
TODO

## 3.5 Arulco Vacations
[Arulco Vacations](http://arulco.blogspot.com/)


# 4 Feature Deep Dive

## 4.1 NCTH
TODO


# 5 Using SVN
TODO

## 5.1 Compiling the game executable
TODO


# 6 Useful links
TODO

- [Bear's Pit community](http://thepit.ja-galaxy-forum.com/)
- Discord link?

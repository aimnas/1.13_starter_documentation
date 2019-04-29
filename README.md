<p align="center">
  <img src="113.png" alt="Jagged Alliance 2 1.13">
</p>

# 0 Intro

## 0.1 Preamble

**WORK IN PROGRESS**

This document is an attempt to create clear and structured starter documentation for people who want to start playing Jagged Alliance 2 v1.13, which will henceforth be referred to as simply "1.13".
From years of hanging around in the [Bear's Pit community](http://thepit.ja-galaxy-forum.com/) we noticed there's a complete lack of explanation how to get started with this mod and everything surrounding it.

This documentation is up to date as of version XXXX.

## 0.2 What is 1.13?

Jagged Alliance 2 v1.13 is a modification for the Jagged Alliance 2 game, with a host of new features and improvements, as well as externalizing a lot of data to make modding easier.  
Lots of features have been added like new resolutions, improved AI, weather effects and new items. 1.13 does still contain the original maps and quests.  
The 1.13 mod has been structured in such a way that it can be used as a baseline for creating new mods.

If you are new to Jagged Alliance 2, 1.13 may be quite overwhelming. This document should help you get started.

## 0.3 List of features
Here are some of the high points:
- Custom resolutions (the original is locked at 640x480).
- Externalisation of hardcoded data and settings to XML and INI files, allowing for deep user customisation and modding.
- AI improvements (e.g. attacking from flanks and using cover)
- A new, very challenging difficulty level: INSANE.
- More detailed IMP (user-created mercenary) customisation, can create multiple IMPs
- Militia can be directly ordered on both the tactical and strategic map
- Weather effects (rain and thunder storms)
- New items
  - Literally hundreds of new guns
  - New armour such as ghillie suits
  - New ammo types, e.g. tracers, match ammo, and cold (subsonic) ammo.
  - New LBE (Load Bearing Equipment, like vests, harnesses and holsters)
  - New weapon attachments ranging from optics to folding stocks to trigger groups.
  - Urban and desert camouflage
- More new game options to fine-tune difficulty and/or playstyle
- New Inventory System makes your mercs' inventories more granular and customisable
- New Weapon Attachment System allowing for up to nine attachment slots
- Mercs from Unfinished Business and Wildfire available
- New keyboard shortcuts and UI features
- [Multiplayer](http://ja2v113.pbworks.com/w/page/4218359/Multiplayer)
- More detailed item descriptions, giving more info about the stats of each item
- Suppressive fire mechanic

...and much, much more.

http://ja2v113.pbworks.com/w/page/4218338/Features

---

# 1 Installation

To play 1.13 you will have to:

1. Acquire and install Jagged Alliance 2
2. Install the 1.13 mod
3. Apply fixes if running Windows 8+

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

This is the preferred way to go for people who want to start playing 1.13 as it will give you a good out of the box experience.  
You can get the latest SCI file from [this OneDrive location](https://onedrive.live.com/?id=13A6926EAC52083!583&cid=013A6926EAC52083).  
If you sort the OneDrive file listing from new to old you should see the file with the highest revision number up on top: download this one.

Once you have downloaded the file you will need to extract its contents with a file archiver. There are different tools to use for this like [7-Zip](https://www.7-zip.org/ "7-Zip homepage").  
Extract the file to the location where your target JA2 installation is located and choose to overwrite files if you get asked, so for this example we'll use `C:\Games\Jagged Alliance 2\`. **If you are not prompted to overwrite files, you did not extract to the correct directory.**

### 1.2.2 Install release 7609

For the special cases with a requirement to run on release 7609 (namely mods), you can find it on the [official 1.13 wiki site](http://ja2v113.pbworks.com/w/page/4218334/Downloads)

### 1.2.3 Install 1.13 from SVN

If you have a special reason to not use the SCI release, for example if you are actively helping to fix bugs in 1.13, it can be handy to get your gamedata and executable from source. This is however an advanced topic which is covered in [section 5](#5-development).

## 1.3 Fixes for newer Windows versions

Technically, there is no need to adjust anything to make 1.13 run well on Windows 7 and older. However there are a few things you will need to do to be able to play 1.13 well on the Windows 8+ versions, here's a list:

- Wine DLLs
- registry fix for 16-bit color mode
- running on one CPU thread

### 1.3.1 Wine DLLs and registry fix

The Wine DLLs and registry fix can be found at `\Docs\Windows Compatibility Fixes\Windows 7-10 Fix.zip`. Make sure to read the included readme!

### 1.3.2 Single CPU thread

To run the game on a single CPU thread, check out [these instructions](https://www.eightforums.com/threads/processor-affinity-set-for-applications-in-windows-8.24086/).

---

# 2 Playing 1.13
TODO
labeled images explaining the HUD in both strategic and tactical views

## 2.1 Starting a new game
TODO

## 2.2 Game settings
TODO

### 2.2.1 New Game Settings

#### 2.2.1.1 Build 8610+

| Setting | Options (default in bold) | Description |
| --- | --- |  --- |
| Difficulty Level | Novice, **Experienced**, Expert, INSANE | This affects: <ul><li>Your starting cash.</li><li>How many Mercs from AIM can die during the game while on assignments (not with you).</li><li>The overall number of troops the Queen can have at one time.</li><li>The number of actions the Queen can make per day.</li><li>The size of patrols.</li><li>The number of Elite troops in patrols.</li><li>The chance of a patrol ambushing you.</li></ul>
| Skill Traits | New, Old | --- |
| Game Style | **Sci-Fi**, Realistic | --- |
| Extra Difficulty | **Save Anytime**, Iron Man | --- |
| Inventory / Attachments | **New/New**, New/Old, Old/Old |  Note there is no Old/New setting as the New Weapon Attachment system can only be used with the New Inventory system. |
| Progress Speed of Item Choices | **Normal** |  --- |
| Available Arsenal | **Tons of Guns**, Reduced |  --- |
| Max. Squad Size | --- |  --- |
| Bobby Ray Quality | 1~10 |  --- |
| Bobby Ray Quantity | 1~10 |  --- |

#### 2.2.1.2 Build 7609 (stable)
Build 7609 has all of the settings from 8610+ (see above), as well as the following (which were moved to `JA2_Options.ini` in build 8610).

| Setting | Options (default in bold) | Setting name in `JA2_Options.ini` (8610+) | Description |
| --- | --- |  --- |  --- |
| Max IMP Characters | --- |  --- |  --- |
| New Chance to Hit System | Off / On |  --- |  --- |
| Enemies Drop All Items | Off / On |  --- |  --- |
| Weapon Overheating | Off / On |  --- |  --- |
| Improved Interrupt System | Off / On |  --- |  --- |
| Inventory Manipulation Costs AP | Off / On |  --- |  --- |

### 2.2.2 In-game settings
TODO

### 2.2.3 Config files
Part of the beauty of the 1.13 mod is just how much control the player has to tailor the experience to their own tastes. This is done via a number of config files.

**Do not use the included INI editor. It is known to cause problems.** To edit INI and XML files, use a text editor. Preferably, one that is more sophisticated than Windows's Notepad, such as [Notepad++](https://notepad-plus-plus.org/).

Regarding directories: wherever you see `\Data-1.13\...`, the `1.13` part should be replaced if playing another mod other than 1.13. e.g. `\Data-AIM\...` for AIMNAS.

#### 2.2.3.1 `ja2.ini`
Found in the root directory (i.e. aside `ja2.exe`). Manages global settings such as resolution and enabling windowed mode.
#### 2.2.3.2 `JA2_Options.ini`
Found in the `\Data-1.13` directory. This is where you will find the bulk of the settings for 1.13.
#### 2.2.3.3 XML Files
Found in the `\Data-1.13\TableData` directory. These files store all sorts of data, such as items, enemy drop tables, NPC inventories, mercenary data, etc. Some files of interest may include `\Items\Weapons.xml`, `DifficultySettings.xml` and `Vehicles.xml`.

## 2.3 Using the new features
TODO

For in-depth details on some of these new systems, please refer to section 4.

- sorting inventories
- keyboard shortcuts
  - grenade launcher angle
  - jumping/vaulting
  - dropping/picking up all backpacks
  - toggle NVG/sunglasses
- spotting for a sniper
- ammo bearing for a machinegunner

## 2.4 Frequently Asked Questions / Starter tips?

### 2.4.1 My New Game settings don't have all the options I recall/have seen elsewhere. Where are they now?
In revision 8610, some of the New Game settings were moved to `JA2_Options.ini`. Refer to [section 2.2.1](#221-new-game-settings) for more info.

### 2.4.2 How do I change the amount of cash I start with?
To change the amount of money you start with, open `\Data-1.13\TableData\DifficultySettings.xml` and edit the `<StartingCash>` value of the difficulty you want to play.

### 2.4.3 What is the difference between OCTH and NCTH?
TODO

#### 2.4.3.1 Tips on actually hitting things in NCTH?
- Optics make a huge difference. Once you secure Drassen airport, consider ordering 2x scopes from Bobby Ray.
- Before optics, consider attacking at night
- Auto fire (and by extension, suppression) is very effective

### 2.4.4 The Drassen counterattack is too difficult!
That's not a question but in `JA2_Options.ini` you can set `TRIGGER_MASSIVE_ENEMY_COUNTERATTACK_AT_DRASSEN` to `FALSE` to disable it.

### 2.4.5 There are so many settings, what should I change first?
[Here are some settings we recommend you take a look at first](settings.md).

### 2.4.6 Who are some good mercs to hire initially?
TODO  
Barry, Buns, Grunty, Igor, Fox, Wolf, Meltdown, Stephen, Grizzly

---

# 3 Mods
Whilst 1.13 is itself a mod, it also has its own mods! Each mod may require a specific version of 1.13 to work.

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

## 3.6 sevenfm's AI fixes
TODO

---

# 4 Feature Deep Dive

## 4.1 NCTH
TODO

## 4.2 NIS/NAS
TODO

---

# 5 Development
The SCI's are made on a two weekly or monthly basis, if however you want to follow the development of 1.13 as close as possible or maybe even help you can compile the executable of 1.13 yourself and combine this with the latest game data.

## 5.1 SVN
The 1.13 development takes place on a so called Subversion server which from here we will call SVN. This software gives developers to possibility to collaborate on the project at the same time without losing any valuable work.  
SVN needs a client to be able to make use of its features, for Windows this client is [TortoiseSVN](https://tortoisesvn.net/downloads.html).

After installing TortoiseSVN you can create a new folder in any place and right click it, the context menu should show you an option called `SVN Checkout...`, when you click this a window will open, read on for further directions.

### 5.1.1 the 1.13 source code
To checkout the 1.13 executable source code with SVN you will have to fill in the following URL of the SVN repository: `https://ja2svn.mooo.com/source/ja2/trunk/GameSource/ja2_v1.13/Build`  
Make sure the value for `Checkout directory` is the directory that you want to place the SVN copy in, leave other settings as they are and press OK.  
The source code repository is just above 1GB in size, depending on your internet speed it could take a while for the SVN data to download, once it's done you will see the message `Completed` at the bottom of the activity window.

### 5.1.2 the 1.13 game data
The game data files are also located in a SVN repository at the following URL: `https://ja2svn.mooo.com/source/ja2_v1.13_data/GameDir`  
Also make sure that the `Checkout directory` is correct and leave the other settings as they are and press OK.  
The game data repository is close to 2GB in size, depending on your internet speed it could take a while to download.

## 5.2 Compiling the game executable
TODO
Jagged Alliance 2 is coded in a mixed style C/C++, the best development environment to use for this is Microsoft Visual Studio, a free version is available at https://visualstudio.microsoft.com/vs/express/
You can pick from many versions of Visual Studio Express like 2005, 2008, 2010, 2013 or 2017

---

#6 Glossary

- Strategic map
- Tactical map
- Bobby Rays
- IMP
- Arulco

---

# 7 Community
- [The Bear's Pit community](http://thepit.ja-galaxy-forum.com/)
- [The Bear's Pit Discord](https://discord.gg/GqrVZUM)

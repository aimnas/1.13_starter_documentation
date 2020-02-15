<p align="center">
  <img src="113.png" alt="Jagged Alliance 2 1.13">
</p>

# Jagged Alliance 2 v1.13 - Play Guide

> **THIS DOCUMENT IS A WORK IN PROGRESS.**

> This documentation is up to date as of 1.13 r8741.

This play guide will provide information about how to use the various features available in 1.13, a UI guide and keyboard shortcuts, information about the many settings available, details about some of the more complex systems, and a few tips to help get started.

> It is strongly recommended to first read the manual to understand how to play the game. It can be found at `Docs\Manuals\JA2_Manual.pdf`. An online version can be found [here](https://store.steampowered.com/manual/545210).

### Contents
- [1. Starting a new game](#1-starting-a-new-game)
  - [1.1 New Game settings](#11-new-game-settings)
- [2. Playing the game](#2-playing-the-game)
- [3. Feature deep dive](#feature-deep-dive)
  - [NCTH (New Chance to Hit)](#ncth)
  - [NIS/NAS (New Inventory System & New Attachment System)](#nis-nas)
- [4. Starter tips](#4-starter-tips)


## 1. Starting a new game
Run `ja2.exe` to boot the game. To start a new campaign, click *Start New Game* on the main menu.

### 1.1 New Game settings
The settings available when starting a new game will vary depending on which release of 1.13 you are using.

#### 1.1.1 Release 8610+

| Setting | Options (default in bold) | Description |
| ------- | ------------------------- | ----------- |
| Difficulty Level | Novice, **Experienced**, Expert, INSANE | This affects: <ul><li>Your starting cash.</li><li>How many Mercs from AIM can die during the game while on assignments (not with you).</li><li>The overall number of troops the Queen can have at one time.</li><li>The number of actions the Queen can make per day.</li><li>The size of patrols.</li><li>The number of Elite troops in patrols.</li><li>The chance of a patrol ambushing you.</li></ul>
| Skill Traits | **New**, Old | The *New* Traits system divides the old Traits into Major and Minor Traits, makes changes, and adds some new Traits as well. Tooltips provide detailed information on what each Trait does by hovering the mouse cursor over it. |
| Game Style | **Sci-Fi**, Realistic | In *Sci-Fi* mode you will encounter a unique enemy type and unrealistic weapons. *Realistic* mode removes these. |
| Extra Difficulty | **Save Anytime**, Iron Man | *Save Anytime* allows you to save... any time you fancy. In *Iron Man* you may only save in a sector not occupied by enemies.  |
| Inventory / Attachments | **New/New**, New/Old, Old/Old |  Essentially, the new systems provide more complexity and customisability. Check [section 3.2](#32-NISNAS) for info. <br /> ※ There is no Old/New setting as the New Weapon Attachment system can only be used with the New Inventory system. |
| Progress Speed of Item Choices | Very Slow, Slow, **Normal**, Fast, Very Fast |  Controls the rate at which better equipment becomes available to both the player and the enemies. For example, if set to *Very Slow*, you will be using pistols and SMGs for a longer period of the game. |
| Available Arsenal | **Tons of Guns**, Reduced |  *Tons of Guns* adds a massive number of guns to the game. If you are not interested in firearms and/or want a a simpler arsenal, pick *Reduced*. |
| Max. Squad Size | 6, 8, 10 |  The available options are dependent on resolution: 640x480 allows for up to 6, 800x600 allows for up to 8, and 1024x768 allows for up to 10. |
| Bobby Ray Quality | 1~10 (**Great (2)**) |  Affects the tiers of guns available in Bobby Ray's shop. [See here](http://ja2v113.pbworks.com/w/page/24219466/Bobby%20Ray) for more information. |
| Bobby Ray Quantity | 1~10x (**Great (2x)**) |  Affects the quantity of the guns available in Bobby Ray's shop. [See here](http://ja2v113.pbworks.com/w/page/24219466/Bobby%20Ray) for more information. |

#### 1.1.2 Release 7609 (stable)
Release 7609 has all of the settings from r8610+ (see above), as well as the following (which were moved to `JA2_Options.ini` in r8610). [See here](http://thepit.ja-galaxy-forum.com/index.php?t=msg&th=23855) for more information.

| Setting | Options (default in bold) | Setting name in `JA2_Options.ini` (r8610+) | Description |
| ------- | ------------------------- | ------------------------------------------ | ----------- |
| Max IMP Characters | **1**~10 |  (deleted as of r8622) |  --- |
| New Chance to Hit System | **Off**, On |  `NCTH` (Default: `FALSE`) |  See [section 3.1](#ncth). |
| Enemies Drop All Items | **Off**, On |  `DROP_ALL` (Default: `0`) |  Controls if NPCs drop all their items when they are killed. |
| Merc Story Backgrounds | Off, **On** |  `BACKGROUNDS` (Default: `TRUE`) |  --- |
| Food System | **Off**, On |  `FOOD` (Default: `FALSE`) |  Enabling the *Food System* means the player must keep their mercenaries fed and quenched else they will suffer drawbacks; potentially death if deprived long enough. |
| Improved Interrupt System | **Off**, On |  `IMPROVED_INTERRUPT_SYSTEM` (Default: `TRUE`) |  --- |
| Inventory Manipulation Costs AP | **Off**, On |  `INVENTORY_MANIPULATION_COSTS_AP` (Default: `FALSE`) |  --- |


## 2. Playing the game

### 2.1 UI
TODO: labeled images explaining the HUD, in both strategic and tactical views, where *1.13* differs from vanilla.

### 2.2 Keyboard shortcuts
A list of all the 1.13 keyboard shortcuts can be found at `Docs\Manuals\JA2_113_Hotkeys.pdf` or [here](http://ja2v113.pbworks.com/w/page/4218351/ja2_and_1_13_hot_keys).

### 2.3 Feature overview
Here are some noteworthy 1.13 features that will be useful.
- http://ja2v113.pbworks.com/w/page/4218346/Instructions%20For%20New%20Features  
- http://ja2v113.pbworks.com/w/page/4218342/HAM%20Features

For in-depth details on some of these new systems, please refer to section 3.

- sorting inventories
- keyboard shortcuts
  - grenade launcher angle
  - jumping/vaulting
  - dropping/picking up all backpacks
  - toggle NVG/sunglasses
- spotting for a sniper
- ammo bearing for a machinegunner

### 2.4 Coolness
https://ja2v113ham.fandom.com/wiki/Game_Progress-Weight_Controls


## 3. Feature deep dive {#feature-deep-dive}

### 3.1 NCTH (New Chance to Hit) {#ncth}
Put simply, NCTH aims to be more realistic by taking into account many more factors when computing the chance to hit. Some players prefer to use OCTH as it is generally more consistent and easier to understand. [This article](https://ja2v113ham.fandom.com/wiki/New_Chance_To_Hit) goes into great detail about how NCTH works.


### 3.2 NIS/NAS {#nis-nas}
TODO

#### 3.2.1 NIS (New Inventory System) {#nis}

#### 3.2.2 NAS (New Attachment System) {#nas}


## 4. Starter tips

### 4.1 Tips on actually hitting things in NCTH
- Optics make a huge difference. Once you secure Drassen airport, consider ordering 2x scopes from Bobby Ray.
- Before optics, consider attacking at night.
- Auto fire (and by extension, suppression) is very effective.

### 4.2 Who are some good mercs to initially hire?
TODO  
Generally, it is very useful to have a decent marksman, a medic and a mechanic around.  
Barry, Buns, Grunty, Igor, Fox, Wolf, Meltdown, Stephen, Grizzly

### 4.3 Basic strategy and tactics for early game
- A merc ending the turn with leftover AP will have a greater chance to trigger an interrupt.
- Lower stances make it harder for a merc to be seen and harder to be hit.
- Make sure your mercs sleep every so often.
- When prone or crouching near cover a merc can "rest their weapon", improving their accuracy.
- When you have captured most of a city, train militia to defend the city while you are elsewhere.
- Suppressive fire reduces the target's AP so it can be very effective.
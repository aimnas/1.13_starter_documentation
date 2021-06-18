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
  - [2.1 UI](#21-ui)
  - [2.2 Keyboard shortcuts](#22-keyboard-shortcuts)
  - [2.3 Feature overview](#23-feature-overview)
  - [2.4 Progress and coolness](#24-progress-and-coolness)
- [3. Feature deep dive](#3-feature-deep-dive)
  - [3.1 NCTH (New Chance to Hit)](#31-ncth-new-chance-to-hit)
  - [3.2 NIS/NAS (New Inventory System & New Attachment System)](#32-nisnas)
  - [3.3 Support roles](#33-support-roles)
- [4. Starter tips](#4-starter-tips)


## 1. Starting a new game
Run `ja2.exe` to boot the game. To start a new campaign, click *Start New Game* on the main menu.

### 1.1 New Game settings
The settings available when starting a new game will vary depending on which release of 1.13 you are using.

#### 1.1.1 Release 8610+

| Setting | Options (default in bold) | Description |
| ------- | ------------------------- | ----------- |
| Difficulty Level | Novice, **Experienced**, Expert, INSANE | Difficulty affects many things: <br />- Starting amount of cash<br />- How many AIM mercenaries can die while on assignments (not with you)<br />- The overall number of troops the Queen can have at one time and the size of patrols<br />- Extra APs for enemies<br />- The number of elite troops in patrols<br />- The chance of a patrol ambushing you<br />- Base chance to hit (if using NCTH)<br /> ※ To see the full effects, look at `\Data-1.13\TableData\DifficultySettings.xml`.
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
| New Chance to Hit System | **Off**, On |  `NCTH` (Default: `FALSE`) |  See [section 3.1](#31-NCTH-New-Chance-to-Hit). |
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

Here are some useful shortcuts added in 1.13 to use in the tactical screen (i.e. combat):

| Shortcut | Function |
| -------- | -------- |
| J | Jump/climb an obstacle with the selected merc. |
| F |	Display useful info about a given tile, including CTH, range, and lighting level. |
| L | Look in a direction. Press L again to ready a weapon. Note that some bonuses, like scope vision range bonuses, only apply when a weapon is raised. |
| Q | Switch between standard grenade launcher angles and higher angles. Higher angles enable you to launch grenades farther and over some obstacles. |
| ALT + R | Reload all weapons (in hand) of selected merc. |
| SHIFT + R | Reload all weapons of your squad. |
| SHIFT + N | Toggle NVGs/sun goggles for all mercs in active team. |
| SHIFT + K | Swap valid weapons between gunsling and primary hand. |
| SHIFT + B | Drop backpacks for all mercs in the current sector. (This can be useful because backpacks reduce merc APs.) |
| CTRL + SHIFT + F | Pick up all dropped backpacks, then sort sector inventory. |

### 2.3 Feature overview
To discover some noteworthy 1.13 features, check out [this page](http://ja2v113.pbworks.com/w/page/4218346/Instructions%20For%20New%20Features). Be sure to look at the links at the bottom.

For information on some of these new systems, please refer to [section 3](#3-feature-deep-dive).

### 2.4 Progress and coolness
As you play the game, a "progress" value increases. As progress increases, items of higher "coolness" become available at shops and in enemy hands. [More info here](https://ja2v113ham.fandom.com/wiki/Game_Progress-Weight_Controls).


## 3. Feature deep dive

### 3.1 NCTH (New Chance to Hit)
Put simply, NCTH aims to be more realistic by taking into account many more factors when computing the chance to hit. Some players prefer to use OCTH as it is generally more consistent and easier to understand. [This article](https://ja2v113ham.fandom.com/wiki/New_Chance_To_Hit) goes into great detail about how NCTH works.

### 3.2 NIS/NAS
These two systems add a lot of new items and customisation options to the game. Note that NAS must be used together with NIS.

#### 3.2.1 NIS (New Inventory System)
If selected when starting a new game, Load Bearing Equipment (LBE) will be available throughout the game to increase the available inventory capacity of your Mercs. These include a selection of Harnesses, Holsters, Packs, Backpacks, and Pouches.

TODO: image comparison

#### 3.2.2 NAS (New Attachment System)
The New Attachment System adds many new attachments, and revises existing ones: 

- Reflex Sights/Match Sights - these attachments make firing your weapon a quick and painless affair. Reflex Sights make the weapon faster to aim. Match Sights increase weapon range slightly but only a few weapons can use them.
- Scopes - these attachments provide a vision range bonus when the weapon is in the raised position. They're available in varying magnification levels. They also have varying degrees of tunnel vision, unfortunately, so make sure you cover your sniper's back! Higher levels magnification will provide a larger vision range bonus, but also have increased tunnel vision effects and require a longer weapon. Therefore not all scopes will work on all guns. In general, a 10x scope will only work with a sniper rifle and a 4x or 7x will work with an assault rifle. Pistols and SMGs typically can only use a 2x, if they can mount a scope at all. 
- Suppressors - these attachments make your weapon more stealthy. A Flash Suppressor eliminates the flash that reveals the shooter's position when firing. Other suppressors (a.k.a. Silencers), available in Pistol, Assault Rifle, and Sniper Rifle sizes, eliminate the flash and also dramatically reduce the weapon's Loudness. However, damage is reduced slightly in exchange.
- Folding & Retractable Stock - Attach these babies to your fixed-stock rifle or SMG and you'll see a reduction in how long it takes to raise your weapon to the ready position. Also makes it a tiny bit harder to hit your target though. Most weapons will only accept one or the other, not both. Many weapons may also have these built in, as depicted in their images.
- Foregrip - Autofire accuracy got you down? Try attaching one of these babies and watch those bullets hit their mark. Again, some weapons may have one built-in, so check your gun's image to see if it has one.
- Trigger Group - Some guns have burst fire, some have autofire, some have both, and some have none. This baby is for those guns without the burst fire... It adds a three round burst fire mode to compatible weapons.
- Laser Aiming Modules - Lasers improve chance to hit but only within a certain range; beyond that they're not much use. They also make your merc more visible to enemies.

TODO: image comparison

### 3.3 Support roles
These functions are optional but can add a nice level of realism or complexity if you desire it.

#### 3.3.1 Spotter
A merc equipped with binoculars can provide an aiming bonus to nearby mercs who are using sniper rifles. [More info here](https://thepit.ja-galaxy-forum.com/index.php?t=msg&th=21603).

#### 3.3.2 Assistant machinegunner
Externally-fed machineguns can be loaded by an adjacent merc holding an ammo belt. [More info here](https://thepit.ja-galaxy-forum.com/index.php?t=msg&th=20084).

#### 3.3.3 Radio operator
Radio sets can be used to call for militia reinforcements, artillery strikes, or jam enemy communications. [More info here](https://thepit.ja-galaxy-forum.com/index.php?t=msg&th=21476).


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

# ENDERAL VR ESSENTIALS (EVRE)
Latest update: November 6th, 2022 (v2.0-Release Candidate 5)

## Table of contents
* [Preamble](#preamble)
* [System Requirements](#system-requirements)
* [Requirements](#requirements)
* [Installation](#installation)
* [Somnium Setup](#somnium-setup)
* [MCM Settings](#mcm-settings)
* [In-Game Settings](#in-game-settings)
* [Updating](#updating)
* [Known issues](#known-issues)
* [Noteworthy mods](#noteworthy-mods)
* [Scoped bows](#scoped-bows)
* [Character Customization](#character-customization)
* [Supersampling](#supersampling)
* [TAA](#taa)
* [Game capture](#game-capture)
* [Language packs](#language-packs)
* [Tools](#tools)
* [Included Mods and Tools (Skyrim VR Installation Folder)](#Included-Mods-and-Tools-Skyrim-VR-Installation-Folder)
* [Included Mods (Mod Organizer 2)](#included-mods-mod-organizer-2)
* [Game Tweaks](#game-tweaks)
* [Nemesis Configuration](#nemesis-configuration)
* [DynDOLOD 3 and SkyVRaan Configuration](#dyndolod-3-and-skyvraan-configuration)
* [Changelog](#changelog)

## Preamble
This guide describes how to configure Skyrim VR to play Enderal: Forgotten Stories SE v2.0.11 in VR using Wabbajack (v2.0.12 is not VR compatible).  Note that the ONLY version of Skyrim you need is Skyrim VR.  The Steam edition of Enderal SE is based off the Skyrim SE engine which does not support VR.  While it is NOT possible to add VR to Enderal SE, Skyrim VR can be "modded" with Enderal SE's files which will allow you to play through the entire game in VR!  (If you wish to play Enderal VR and Skyrim VR simultaneously, you will need to mod each game seperately using either two seperate installations of Mod Organizer 2 OR two copies of your Skyrim VR folder.)

While you can optionally download and configure all the [recommended mods](#Included-Mods-and-Tools-Skyrim-VR-Installation-Folder) manually through Mod Organizer 2, Wabbajack simplifies the process of downloading all the required Skyrim VR mods and patches necessary to play Enderal SE in VR to a single click.  This guide uses a lightweight modlist designed to deliver an optimal VR experience with minimal performance loss.  Most of the included mods are simple texture mods which can be safely disabled at any time if you prefer an even lighter loadout with vanilla textures.  This modlist was optimized for Virtual Desktop and Air Link and should perform extremely well when playing the game wirelessly. 

Special thanks to the Enderal SE modding team, Scenic Route Games, and sasa2727 for the VR patch which made this guide possible!

## System Requirements
Minimum:
* CPU: Intel Core i5-6600K or AMD Ryzen 5 1400 or better
* RAM: 8 GB
* OS: Windows 7/8.1/10 (64-bit versions)
* GPU: Nvidia GeForce GTX 970 / AMD RX 480 8GB or better
* STORAGE: 178GB (178GB needed for installation, 114GB needed post installation)

Recommended:
* CPU: Intel Core i7-4790 or AMD Ryzen 5 1500X or better
* RAM: 8 GB
* OS: Windows 10 (64-bit versions)
* GPU: Nvidia GeForce GTX 1070 8GB or better
* STORAGE: 178GB (178GB needed for installation, 114GB needed post installation)
* WI-FI: 802.11ac or 802.11ax (for Virtual Desktop or Air Link; optional) 

## Requirements
* [The Elder Scrolls V: Skyrim VR](https://store.steampowered.com/app/611670/The_Elder_Scrolls_V_Skyrim_VR/)
* [Enderal: Forgotten Stories (Special Edition)](https://store.steampowered.com/app/976620/Enderal_Forgotten_Stories_Special_Edition)
* [Premium NexusMods account](https://www.nexusmods.com/)
* [Wabbajack](https://www.wabbajack.org/#/)
* [EVREv2.0-RC5.wabbajack](https://github.com/Ashok0/EnderalVREssentials-Nightly/releases)
	
## Installation
1.  Add Enderal SE to your Steam library from [HERE](https://store.steampowered.com/app/976620/Enderal_Forgotten_Stories_Special_Edition/). The game needs to be in your Steam library but does not need to be installed.
2.  Install a clean copy of Skyrim VR from [HERE](https://store.steampowered.com/app/611670/The_Elder_Scrolls_V_Skyrim_VR/).
	* If you already have a pre-modded Skyrim VR folder and do not wish to uninstall the vanilla game, you can rename your \SkyrimVR\ folder and then redownload a second clean copy of the game from Steam by reverifying the files.  You can then use one copy of the game to continue playing Skyrim VR along with a second copy of the game for playing Enderal VR.
3.  Run Skyrim VR one time from Steam and then exit the game.
4.  Login to [Nexusmods.com](https://users.nexusmods.com/auth/sign_in) using a Premium login.
5.  Download Wabbajack v3.x from [HERE](https://www.wabbajack.org/#/). Place the files in a blank folder i.e. C:\Games\Wabbajack and run the program one time. 
6.  Create a new folder where you wish to install Enderal VR i.e. C:\Games\Enderal VR
7.  Download "EVREv2.0-RC5.wabbajack" from [HERE](https://github.com/Ashok0/EnderalVREssentials-Nightly/releases) and place it anywhere outside of your Wabbajack folder.
8.  Launch Wabbajack and select "Install from Disk".  Next, manually select the *.wabbajack* file under "Target Modlist".  **Do not attempt to install Enderal VR Essentials by double-clicking the .wabbajack file directly or the Wabbajack installation will fail with an error related to "\Extractors\windows-x64\7z.exe".**
9.  Under "Modlist Installation Location", select the folder you created above under Step 6.  Tick "Overwrite Installation" if you are updating a previous installation and then click the green "PLAY" icon in the lower right. 
10.  Wait for Wabbajack to download all the mods and patches required to play Enderal VR.  This could take several hours depending on your Internet connection.
		* If you receive an error message during this step, a mod has most likely been updated preventing the modlist from installing.  Wait for me to update this Wabbajack modlist and then try again.

11. Once Wabbajack is done downloading and configuring Enderal VR, navigate to your game folder from Step 6.
12. Copy the contents of \Game Folder Files\ to C:\Program Files (x86)\Steam\steamapps\common\SkyrimVR
13. Launch Mod Organizer 2. 
14. Select a game profile in the upper left drop down bar.  You can select 3 different options:
* **Enderal VR Essentials**: *This profile will give you an experience that is similar to the vanilla game. Gameplay mechanics are untouched outside of VR mods.*
* **Enderal VR Essentials - Enderal Gameplay Overhaul**: *This profile completely overhauls the gameplay mechanics of Enderal with Ixion XVII's EGO mods. This includes a ton of balance changes, improvements to the AI, new gameplay mechanics, new weapons/spells/potions and much more.*
* **Enderal VR Essentials - Somnium Overhaul**: *This profile contains all the features from the EGO profile along with an expansive new Enderal mod, "Apoapse’s Apparel", which was created by Scenic Route Games.  Scenic Route Games has hand-replaced every outfit and weapon in the game, as well as the majority of the other assets, to best achieve a more modern view of the Enderal worldspace.  This overhaul also replaces the main menu music with a newly composed theme from Scenic Route Games.  An end game fight is replaced with a more morally grey decision you have to make, and the whole scene is streamlined without cutting out the quality of the dialogue and exposition.* (**The Somnium assets have been temporarily removed at the request of Scenic Route Games.  They will be added back at a later date with official support from the original developer.  In the interim, perform the [following steps](#somnium-setup) to use the optional Somnium profile.**)
15. Configure your mod loadout in Mod Organizer 2: 
	* Tick "*Enable TAA FX*" to enable TAA effects.  While this reduces shimmering, it is NOT recommended to enable TAA effects as this breaks parallax textures. (There is a seperate TAA setting in-game which must always be enabled for menu artwork to display properly in VR.)
	* Tick "*Clear HUD VR*" to hide Health, Magicka, Stamina bars, the Sneak Indicator, and Enchantment Charges.
	* Tick "*Vanilla HUD Size for VR*" if you wish to increase the size of the HUD.
	* Tick "*VRIK Rift-Index-WMR Controller Bindings*" if using a Rift, Valve Index, or WMR headset.
	* Tick "*Vanilla Cubemaps for Darker Water*" to enable optional cubemaps without reflections for darker nighttime water.	
	* Tick "*Equippable Tattoo Skins UNP + CBBE*" if you wish to apply tattoos/bodypaint to your character (female only).	
	* Tick "*Replace spiders with wolfs and bears*" OR "*Arachnophobia - No Spiders and Beetles*" if you have arachnophobia!  Choose only one.
	* Tick "*Story Mode*" to enable gameplay tweaks to make the game enjoyable without worrying about micromanaging and difficulty. (If "Story Mode" is enabled with the Somnium Overhaul profile, EGO mods are effectively disabled.  This allows you to enjoy the Somnium outfits and weapons without worrying about the added difficulty from EGO mods).
	* Tick "*DynDOLOD_Output_PERFORMANCE*" OR "*DynDOLOD_Output_QUALITY*".  Select only one.  The PERFORMANCE version uses "billboard1" trees for LOD4 for optimal performance.  The QUALITY version uses "level0" trees for LOD4.  This will greatly improve tree LODs but results in -10fps in large open areas on an RTX 3070.  The PERFORMANCE version is enabled by default.
16.   (Optional) You can optimize your VR performance by installing either [VR Performance Toolkit](https://github.com/fholger/vrperfkit) (Compatible with all headsets) or [Skyrim VR OpenComposite](https://www.nexusmods.com/skyrimspecialedition/mods/85389/?tab=files) (Compatible with Oculus headsets only, highly recommended when using Air Link. Make sure to install [OpenXR](https://mbucchia.github.io/OpenXR-Toolkit/) as well). Put the 64-bit openvr_api.dll to your Skyrim VR installation folder. Backup and overwrite the existing DLL file in your Skyrim VR folder.  
		* OpenComposite improves framerates by launching Enderal VR directly through the Oculus runtime and eliminating overhead from Steam VR.
17.   (Optional) You can delete the \downloads\ folder in your Mod Organizer 2 folder to remove downloaded mods which are only needed during installation.  This will free up 58GB of hard disk space.
18.   Make sure "SKSE" is selected in the upper right dropdown bar and click "Run" to launch and play Enderal VR!  
		* You can optionally click "Shortcut" underneath "Run" to create a shortcut for launching Enderal VR directly from the Windows desktop!

## Somnium Setup
The Somnium assets have been temporarily removed at the request of Scenic Route Games.  They will be added back at a later date with official support from the original developer.  In the interim, perform the following steps to use the optional Somnium profile: 
1. Install Somnium from the official website [**HERE**](https://www.scenicroute.games/projects/somnium).
2. Copy the following files from Somnium to the corresponding mod folders in the Enderal VR Essentials installation location: 

- \Apoapse's Accoutrement\meshes\ and \Apoapse's Accoutrement\textures\
- \Screw the Black Guardian v2\Scripts\, \Screw the Black Guardian v2\Sound\, and \Screw the Black Guardian v2\Video\
- \Somnium Music Edits\Music\
- \Somnium Retextures\meshes\ and \Somnium Retextures\textures\

## MCM Settings
Once you start a new game, you can configure your individual Enderal VR mods through the in-game Mod Configuration Menu (MCM) which is accessible under System > Mod Configuration.  All MCM settings are pre-configured for a good VR experience but following changes are suggested:

* R.A.S.S:  Select Options > Raining and set this option to "Off" if you dislike waterdroplet effects on the camera when it is raining.

## In-Game Settings
1. Under System > Settings > VR Performance > Object Fade, set "Object Fade" to 0% to significantly improve performance in large outdoor areas.  This is the most resource intensive setting for Enderal VR. (Set to 40% by default to reduce pop-in effects when walking around).
 
## Updating

This Wabbajack modlist will be updated regularly with the latest versions of all its included mods.  If the Wabbajack is updated, just re-download [EVREv2.0-RC5.wabbajack](https://github.com/Ashok0/EnderalVREssentials-Nightly/releases) and re-install the Wabbajack file to keep your mods up to date with a single click.  Be sure to set the "Installation Location" to the same path used during the original installation and tick "Overwrite Installation" before hitting the "Run" button.  Updating should be much quicker than the initial installation process.    

Wabbajack will delete all files that are not part of its modlist when updating!  Your downloads folder will not be touched.  If you have installed additional mods not included in the Wabbajack, you will need to re-install them manually if you choose to update your mods via the Wabbajack file.  You can alternatively update your mods manually through Mod Organizer 2.

## Known issues (Moderate)
* Your headset and controllers must be active before launching the game or it will not start.
* Cutscenes do not work.  Audio always plays against the SteamVR backdrop or hourglass logo (when using Open Composite). This is a very minor issue as there are only 3 cutscenes in the entire game.  These can be easily viewed on YouTube and two of the videos are introduction videos which play at the beginning of the game.
* You have no body or hands during the tutorial.  This is normal as you do not get an avatar until completing the character creation wizard.
* There are some clipping issues with the character creation wizard on the ship.  You may need to step through the wall of the ship or peer above the ship ceiling to view the full menu.
* :small_orange_diamond: Do not press any triggers during conversations with NPCs.  There is a nasty bug where interrupting dialogue may prevent you from finishing key conversations and will soft lock your game.  The only way to continue is to reload an old save game. :small_orange_diamond:
* :small_orange_diamond: If you get stuck in Duneville and are unable to move, enter the following in the console: player.setscale 1 :small_orange_diamond:
* :small_orange_diamond: After going down the lift at the Aged Man's Manor, you must immediately save/reload your game at the bottom of the elevator or the VRIK mod will break. :small_orange_diamond:
* If you get stuck during quests from animations that do not trigger properly, press "~" with the game in focus on your monitor and type player.tai or enableplayercontrols in the console.
* The werewolf race has issues in Enderal VR so avoid using the lycanthropy tree perk.

## Known issues (Minor)
* If you are using Air Link, it is recommended to keep your headset at 72Hz due to known latency issues with Oculus firmware V43.
* If you are using Virtual Desktop, you may see a subtle "rectangular box" around the edges of the view where the image becomes blurry outside of the rectangle.  This effect is normal and is caused by the foveation used by Virtual Desktop when streaming Enderal VR wirelessly.
* Loading saved games during the opening tutorial may cause VRIK to glitch out.
* If you need to reset your height in-game, do not run "Floor Fix" through Open VR Advanced Settings as this may causes problems with VRIK where you get stuck in "Sneak" mode.  Recalibrate your height through the VRIK Calibration Power.  You can do this by selecting the VRIK Calibration Power from the magic menu.
* There are physics issues with shattered glass.
* If you have trouble selecting ingredients at alchemy benches, on your left controller be sure to tap the analog stick to the right which should allow you to select ingredients for crafting.
* If you have issues equipping arrows for your bow, you need to reach behind your back in real life to grab an arrow.  This is a feature from the included Simple Realistic Archery mod. 
* If the Hero menu doesn't pop up when raising one controller over your head, make sure the Enderal window is active and in focus on the Windows desktop.
* The Unique Sets Replacer SE mod significantly improves many Enderalean armor sets but some armor pieces may cause an invisible wrist glitch.  This is typically not noticable when you are wearing gauntlets.
* Steam achievements do not work.
* Crouching in real life will cause a minor "hitch" in your video as you approach the ground.  This is due to the "Automatic Sneaking" feature which is enabled by default.  If you dislike this effect and don't care about physical sneaking, you can turn this feature off from the in-game settings.
* By default, your shield is slightly offset from your hand position when equipped.  This can be fixed by enabling "Realistic Shield Grip" from the in-game settings, but when this feature is enabled you cannot walk forward/backward when your shield is raised if you are using Wand-Relative locomotion.
* The talent points in the game are too high to reach in VR.  To use them, install [OVR Advanced Settings](https://github.com/OpenVR-Advanced-Settings/OpenVR-AdvancedSettings) which allows you to change your player height on the fly.  From the in-game Steam menu, select OVR Advanced Settings > Space Offsets -> Y-Axis (up/down). Just lower the value there to "grow" ingame. Note that this fix requires SteamVR and is not compatible with OpenComposite.
* If using Auriels Holy Bow - REDUX, Blended Roads, Embers HD, Embers XD, Glorious Doors of Skyrim (GDOS) SE, Inferno - Fire Effects Redux, JS Instruments of Skyrim SE, Kanjs - Chaurus Eggs and Staff, Skyrim Particle Patch for ENB, Snazzy Furniture and Clutter Overhaul SE, Static Mesh Improvement Mod - SMIM, Dibella Statue, Unofficial Skyrim Special Edition Patch, or Water for ENB you must make sure you are NOT using any plugins for these mods.  Only meshes and textures may be used.  Delete ALL .esp files associated with these mods before launching the game or running DynDOLOD 3.0. (Incompatible plugins have already been removed with this Wabbajack release.) 
* If newly installed or updated mods contain Tamriel worldspace data, the .esp plugin must be fixed by removing all Cell and Worldspace data for Tamriel in xEdit.  Failure to do so will result in DynDOLOD 3.0 crashing and may cause game breaking bugs. (All plugins have already been fixed with xEdit with this Wabbajack release.) 
* When using OpenComposite, you cannot have any audio recording devices attached to your PC aside from your VR headset or Dragonborn Speaks Naturally will not work. 
* With the exception of texture/mesh mods, mods cannot always be safely removed mid-savegame.



# YOU'RE ALL DONE!  ENJOY ENDERAL: FORGOTTEN STORIES IN VR!  ALL STEPS BEYOND THIS POINT ARE OPTIONAL.



## Noteworthy mods
[**Enderal SE**](https://www.nexusmods.com/enderalspecialedition/mods/1?tab=files): Complete Enderal for Skyrim Special Edition.

[**Enderal VR - Patch**](https://www.nexusmods.com/enderalspecialedition/mods/8?tab=files): This mod offers you the opportunity to play Enderal in VR. Supports special gestures when your Skyrim VR window is active in the forefront in Windows.  Raising your right controller above your head will bring up the Hero menu.  Repeating this gesture will close the Hero menu.  Raising your left controller above your head will teleport you to the Akropolis.   

[**Dear Diary VR - Paper SkyUI and Categorized Favorites**](https://www.nexusmods.com/skyrimspecialedition/mods/44874?tab=files): Replacer for Skyrim interface in a paper style.  Disable if you prefer the classic SkyUI interface.

[**VR Menu Mouse Fix**](https://www.nexusmods.com/skyrimspecialedition/mods/33414?tab=files): Enables mouse for SkyUI-VR. You can use your VR controllers to control the menu cursor like a laser pointer.

[**Smaller HUD for VR Larger Text Patch**]: [Smaller HUD for VR](https://www.nexusmods.com/skyrimspecialedition/mods/30726?tab=files) is a simple mod that reduces the size of the HUD elements and text by about 50% for added immersion.  This mod makes the HUD extremely VR friendly but it also makes text a bit difficult to read.  The Larger Text Patch will increase text size while retaining the smaller HUD elements from the original mod.

[**RaceMenu**](https://www.nexusmods.com/skyrimspecialedition/mods/19080?tab=files): A complete overhaul to the character creation menu.  Allows you to customize your avatar and load custom character "presets".  A fun mod if you want to take pictures of your character in VR using the VRIK "Selfie Mode".  The RaceMenu window appears once after the opening mission and can be accessed any time in-game through the console.  Press ~ to access the console.  Enter showracemenu and hit ENTER to bring up the RaceMenu window and then press ~ to exit the console.

[**VRIK**](https://www.nexusmods.com/skyrimspecialedition/mods/23416?tab=posts): VRIK will display the player character's body in SkyrimVR and animate it to match your movements. Weapons can be kept, drawn, and sheathed in up to 14 visible holsters on your body.  Spells can be cast by simply opening your hands when using Index controllers or Touch controllers with grips (Kiwi grips recommended).

[**VRIK Rift-Index-WMR Controller Bindings**](https://www.nexusmods.com/skyrimspecialedition/mods/23416?tab=files): These control bindings are an optional add-on for VRIK to make it easier to use holsters.  These bindings are disabled by default but MUST be enabled if you are using Index controllers.

[**VRIK Neardistance Fix Patch for Build**](https://mega.nz/file/fABDEKBL#6hMat5Urx2QkCNB7Z_-PCFYC3YPLcoTYJLvq3sgcMMA): Sets fNearDistance to 13 to fix mountain flickering.

[**HIGGS VR**](https://www.nexusmods.com/skyrimspecialedition/mods/43930?tab=files): Hand collision, physics object grabbing, and gravity gloves-style mechanics for Skyrim VR.

[**PLANCK - Physical Animation and Character Kinetics**](https://www.nexusmods.com/skyrimspecialedition/mods/66025?tab=files): Physically-driven animation in Skyrim. Characters interact with physics and can be grabbed, melee hit detection is physically accurate, and much more.

[**Spell Wheel VR**](https://www.nexusmods.com/skyrimspecialedition/mods/47630?tab=files): Selection wheel mod for Skyrim VR. It allows you to select spells, weapons, shields, arrows, potions, poisons, food, torch, armors and more without going into a menu very quickly by press of a button or button combinations to spawn the wheel and hold your hand over the item and letting go of the button. It's equipped automatically.  Be sure to set the "Slow Time Scale" to 5 in the Spell Wheel VR MCM if you want a nice slow motion effect when selecting items from the spell wheel.  Set "Presets" to Spellsword in the Spell Wheel VR MCM to make spells and weapons selectable from the spell wheel.

[**Wearable Health Bars - Soul Gauge**](https://www.nexusmods.com/skyrimspecialedition/mods/65737?tab=files): Jewelry that displays Health, Magicka, Stamina, enchantment charge, or equipped ammo count on your hands. Glows in the dark!

[**Spellsiphon - Complete Edition**](https://www.nexusmods.com/enderalspecialedition/mods/357?tab=files): Experience gameplay focused on combos and synergy. Lessen the need for menus or hotkeys through a system where swapping spells and weapons is streamlined and rewarding. Continue the fight at 0 magicka by using new spell types. Enjoy a plethora of new sounds and visual effects. Grow in power by playing skillfully, not just from levels and gear.

[**Magic Improvements for Skyrim VR**](https://www.nexusmods.com/skyrimspecialedition/mods/55751?tab=files): Vastly improved dual casting, spell effect size scales based on magicka percentage, and additional options for aiming spells in VR.

[**NavigateVR**](https://www.nexusmods.com/skyrimspecialedition/mods/47174?tab=files): This mod brings immersive navigation to VR with a functional compass which is automatically added to your inventory.  While this mod does support equippable in-game maps, there are no available maps for Enderal locations. Replaced default Riften map with a map of Ark from "Anna's Enderal Map" mod to keep the map artwork lore friendly to Enderal.

[**Splashes of Skyrim - VR**](https://www.nexusmods.com/skyrimspecialedition/mods/47710?tab=files): SKSE plugin that adds projectile based water splashes and ripples, and underwater explosions.

[**DragonbornSpeaksNaturally**](https://www.nexusmods.com/skyrimspecialedition/mods/16514?tab=files): Adds speech recognition to Skyrim VR or Skyrim SE so you can recite your dialogue lines to select them.  Requires no speech training!

[**Immersive Gathering (Woodchopping and Mining) SE - VR Friendly**](https://www.nexusmods.com/skyrimspecialedition/mods/29710?tab=files): Chop wood and mine ore for real by swinging your axe or pickaxe!

[**HapticSkyrimVR - Spellcasting and Enhanced Bow and Melee Feedback SKSE Plugin**](https://www.nexusmods.com/skyrimspecialedition/mods/20364?tab=files): SKSEVR plugin to get spell casting and enhanced bow and melee haptic feedback on VR controllers.

[**Simple Realistic Archery VR**](https://www.nexusmods.com/skyrimspecialedition/mods/28524?tab=files): Automatically unequips your arrows after shooting them, then reequips the arrow after pressing the trigger (MCM configurable) over your shoulder. It also has options for binding different arrows to different buttons, for the position and size of the quiver, and options for attribute costs. Up to 25 arrow types can be bound at once.

[**Weapon Throw VR**](https://www.nexusmods.com/skyrimspecialedition/mods/31374?tab=files): Allows you to throw your equipped weapons in VR by holding a button, swinging your hand, and releasing it. All six melee weapon types, shields and torches are supported. Supports vanilla and mod added weapons. Includes Auto-Return and Auto-Aim features. Comes with an MCM to configure every setting.

[**Dual Wield Block VR**](https://www.nexusmods.com/skyrimspecialedition/mods/28456?tab=files): SKSE plugin to let the player block attacks while dual wielding (two weapons or weapon + spell) or unarmed.

[**LocationalDamageSKSE VR**](https://www.nexusmods.com/skyrimspecialedition/mods/26447?tab=files): Locational Damage for SKSE VR! Do extra damage depending on which body part you hit with your arrows or spells.

[**No Stagger Mod**](https://www.nexusmods.com/skyrimspecialedition/mods/16335?tab=files): This mod makes your character unstaggerable.  This prevents you from being stunned in combat and having a bright light flash across your vision.

[**Sprint Jump VR**](https://www.nexusmods.com/skyrimspecialedition/mods/28354?tab=files): An SKSE plugin to allow Sprint Jumping in SkyrimVR. Increase sprint jump height and distance with a multiplier in the config file.

[**Scoped Bows SE**](https://www.nexusmods.com/skyrimspecialedition/mods/912?tab=files): Scoped Bows is a huge weapons mod that adds scoped variants of all bows to the game, designed to be used without crosshair.  You MUST disable "Adjust Held Weapons Position" in the VRIK MCM or aiming through scopes will not work properly.

[**Simple Iron Sights for Sighted Crossbows VR**](https://www.nexusmods.com/skyrimspecialedition/mods/38946?tab=files): Changes the sights included in Sighted Crossbows VR into more of a simplistic, medieval style.  A great mod to use in combination with HIGGS which now allows crossbows to be used as two handed weapons.

[**Blocking and Flash VR**](https://www.nexusmods.com/skyrimspecialedition/mods/74463): Block Sparks & Impact Sounds for Skyrim VR without affecting gameplay.

[**HLP Night Sky High**](https://www.nexusmods.com/skyrimspecialedition/mods/8752) and [**STO - Stars 4K Only small stars**](https://www.nexusmods.com/skyrimspecialedition/mods/4931?tab=files): These two mods are extremely underrated gems which greatly improve nighttime scenes in VR with realistic lore-friendly night sky textures.  These mods use very small stars which greatly reduces SDE in VR which tends to be a problem with other night sky mods as stars have very high contrast and are drawn very far in the distance.  You can use both of these mods together or you can use one or the other for slightly different effects.  Both night sky mods are enabled by default.  

[**HD Transparent Smaller Snowflakes 2K**](https://www.nexusmods.com/skyrim/mods/74048?tab=files): This mod replaces the default Skyrim snowflakes with Ultra HD Ultra Realistic Transparent Crystal Snowflakes. 

[**Caliente's Beautiful Bodies Enhancer - CBBE**](https://www.nexusmods.com/skyrimspecialedition/mods/198?tab=files): Pre-installed using "Vanilla" body shape with "NeverNude" underwear options.  Improves meshes and textures for your body and hands and gives female NPCs a more feminine form while retaining a lore-friendly Enderal aesthetic. 

[**Equippable Tattoo Skins UNP + CBBE**]: Disabled by default.  For female players only.  If enabled, this mod allows you to craft up to five unique tattoos at a forge which you can apply to your body from your inventory.  These tattoos are NOT lore friendly but you can overwrite these tattoos in your \mods\Equippable Tattoo Skins UNP + CBBE\textures\actors\character\equipskins\female\ folder with custom bodypaint textures of your choice.  Bodypaint applied to female characters with this mod can be viewed in first person on your VRIK body when playing in VR!

[**R.A.S.S - Rain Ash And Snow Shader**](https://www.nexusmods.com/skyrimspecialedition/mods/22780?tab=files): "R.A.S.S." adds weather effects to the Player such as water droplet and cold breathe effects in your vision. You can optionally disable select weather effects from the R.A.S.S. MCM. 

[**Conduit - Short-term Weapon Infusions**](https://www.nexusmods.com/skyrimspecialedition/mods/58023?tab=files): When holding a weapon in one hand and a spell in the other, you are able to temporarily "conduct" the spell through that weapon. Different categories of spells make the weapon do different things. This effect will overlay on top of normal enchants and does include additional weapon FX that will overlay too. It even works on Bound weapons.

[**Dirt and Blood - Dynamic Visual Effects**](https://www.nexusmods.com/skyrimspecialedition/mods/38886?tab=files): Your character will accumulate dirt and blood dynamically, which you can clean by swimming or standing in the rain. The effects are mostly visual only and do not affect gameplay. NPCs will also get bloody as a result of battles. Mod is designed to be simple and lightweight.

[**Frozen Electrocuted Combustion**](https://www.nexusmods.com/skyrimspecialedition/mods/3532?tab=files): Applies visual effects to NPCs and the player, when killed by air, ash, dragons, drain, fire, frost, fear, lightning, poison, soultrap, steam and sun damage status effects.

[**Replace spiders with wolfs and bears**](https://www.nexusmods.com/enderalspecialedition/mods/31?tab=files): Replaces spiders with wolves and bears.  Enable if you have arachnophobia! 

[**DynDOLOD**](https://www.nexusmods.com/skyrimspecialedition/mods/32382/?tab=files): Adds distant LOD for objects and trees to Skyrim.  When looking across the horizon in large open areas, this mod allows you to see FAR more detail than what is possible with the vanilla game, even with in-game LOD settings set to max.

[**SkyVRaan - Shimmering VR Waters**](https://www.nexusmods.com/skyrimspecialedition/mods/30571?tab=files): Adds a fake reflection effect to Skyrim VR's outdoor water. It breaks up the distant LOD, shows wave movement on the distant water, and gives an illusion of water depth in the distance. Also has improved realism and clarity of near water.


## Scoped bows
* For scoped bow aiming to work, open VRIK MCM and disable "Adjust Held Weapons Position" (This setting has been pre-configured with this Wabbajack release.)
* You can add scoped bows to your inventory by pressing "~" with Enderal VR active on your Windows desktop and entering one of the following lines:

    * Player.AddItem 1801FE36 1 (Dwarven Sniper)
    * Player.AddItem 18033A62 1 (Dwarven Sniper Prototype)
    * Player.AddItem 1801FE32 1 (Daedric Wrath)
    * Player.AddItem 1801FE4C 1 (Nordic Assault Bow)
    * Player.AddItem 1801FE58 1 (Dragonbone Bow - Scoped)
    * Player.AddItem 1801FE4F 1 (Glass Bow - Scoped)
    * Player.AddItem 1801FE54 1 (Hunting Bow - Scoped)
    * Player.AddItem 18033257 1 (Noble Hunting Bow - Scoped)
    * Player.AddItem 1801FE47 1 (Imperial Bow - Scoped)
    * Player.AddItem 1800FB08 1 (Orcish Bow - Scoped)
    * Player.AddItem 18019D0E 1 (Elven Bow - Scoped)
    * Player.AddItem 1800FB03 1 (Stalhrim Bow - Scoped)
    * Player.AddItem 18023F40 1 (Ebony Bow - Scoped)
    * Player.AddItem 1802E14F 1 (Forsworn Bow - Scoped)
    * Player.AddItem 1802E145 1 (Longbow - Scoped)
    * Player.AddItem 1802E151 1 (Nord Hero Bow - Scoped)
    * Player.AddItem 1802E14A 1 (Falmer Bow - Scoped)
    * Player.AddItem 1803365D 1 (Ancient Nord Bow - Scoped)
    * Player.AddItem 18033660 1 (Supple Ancient Nord Bow - Scoped)
    * Player.AddItem 1804CB2C 1 (Imperial Legionary Bow)
    * Player.AddItem 1804CB28 1 (Stormcloak Hunting Bow)
    * Player.AddItem 02000800 1 (Auriel's Bow)
    * Player.AddItem 04018ED5 1 (Glass Bow of the Stag Prince)
    * Player.AddItem 460012C8 1 (Unbound Bow)
    * Player.AddItem 0402C01A 1 (Dwarven Black Bow of Fate)
    * Player.AddItem 000CC392 1 (Angi's Bow)
    * Player.AddItem 000AB705 1 (Bow of the Hunt)
    * Player.AddItem 0200CFB6 1 (Zephyr)
    * Player.AddItem 000F652C 1 (Nightingale Bow)
    * Player.AddItem 00017059 1 (Firiniel's End)
    * Player.AddItem 18005902 1 (Drainspell Bow)
    * Player.AddItem 000F5D22 1 (Gauldur Black Bow)
    * Player.AddItem 000C0186 1 (Froki's Bow)
    * Player.AddItem 0006B9AD 1 (Dravin's Bow)
    * Player.AddItem 1801FE32 1 (Daedric Wrath)

## Character Customization
### RaceMenu Presets
You can customize your character's appearance any time in-game by pressing "~" to access the console and entering:  showracemenu.  Note that you should never change your Race or you will lose all your stats.  While your appearance is mostly irrelevant in VR, it can be fun to customize your avatar if you wish to take selfies in VR using the VRIK "Selfie Mode".

If you wish to use a custom RaceMenu Preset, perform the following steps:
1. Download the RaceMenu Preset you want from NexusMods and place any ".jslot" files in C:\Program Files (x86)\Steam\steamapps\common\SkyrimVR\Data\SKSE\Plugins\CharGen\Presets\.  (You will need to create these folders manually.)
2. Install any prerequisite mods for your RaceMenu Preset through Mod Organizer 2.
3. Launch Enderal VR 
4. Once you are in-game, press ~ to access the console.  Enter showracemenu and hit ENTER to bring up the RaceMenu window and then press ~ to exit the console.
5. Click the "Presets" tab in the right panel and then select "Load Preset" on left panel and click the .jslot file for your RaceMenu Preset.   
6. If your RaceMenu Preset uses High Poly Head, select the "Sliders" tab in the right panel > Select "Head" in the top navigation bar in the left panel > Click "Face Part" in the menu below > Tap your analog stick to the right to select the "High Poly Head" version of your RaceMenu Preset.  This will give you a much higher quality face with no jaggies!
7. Select Done > Close > Done
8. To view your avatar, navigate to the in-game menu and select System > Mod Configuration > VRIK > Controls > Tick "Selfie Mode"
9. Return to your game and raise your right hand in the air to enter and exit "Selfie Mode".  You can now see your avatar in third person for taking selfies in VR! 

### Bodypaint
If you like bodypaint, you can actually customize your character with bodypaint and view your bodypaint in VR on your VRIK body.  You cannot apply bodypaint through RaceMenu, however, as RaceMenu treats paint as overlays which won't work properly with VRIK.  To use bodypaint, you need to apply the paint directly to your player's skin texture file using the "Equipable Female Tattoo UNP CBBE" mod.  You can do this through the following steps (female only):
1. Download a CBBE bodypaint mod of interest from NexusMods.
2. Unpack the contents and then extract the contents of the .bsa files with [Bethesda Archive Extractor v0.10](https://www.nexusmods.com/skyrimspecialedition/mods/974?tab=files). 
3. Open the \textures\ folder from the extracted .bsa files and select a .dds file with the bodypaint you wish to use.  Open this file in Adobe Photoshop.  Select Image > Image Size > Set the Width and Height to 2048px and click OK. 
4. Navigate to the \mods\Bijin skin UNP and CBBE\ folder in your Mod Organizer 2 folder.  Search for "femalebody_1.dds" and open this file in Adobe Photoshop. 
5. Select the Photoshop tab with the bodypaint image, then select the entire image with the Rectangular Marquee Tool and then hit Edit > Copy Merged.  
6. Select the Photoshop tab with the Bijin skin image, then hit Edit > Paste.  Save this file in the following location in your Mod Organizer 2 folder: \mods\Equippable Tattoo Skins UNP + CBBE\textures\actors\character\equipskins\female\ and overwrite the existing tattoo1.dds file (Do not overwrite your original file or all NPCs will have warpaint applied to their skin!).  
7. Finally, enable "Equippabe Tattoo Skins UNP + CBBE" in Mod Organizer 2 and launch the game! 
8. Travel to a forge and craft your warpaint as a tattoo.  Bodypaint will be added to your inventory where you can apply it to your body in VR and successfully view it on your VRIK body!

### Custom Armor
You can further customize your character in VR with custom armor mods.  Custom armor mods work fine in Enderal VR with VRIK and HIGGS but most custom armor needs to be spawned into your inventory using the armor item codes via the console.  You can install custom armor and locate their item codes manually by performing the following steps below.
1. Download the custom armor mod of your choice from [NexusMods](https://www.nexusmods.com/skyrimspecialedition/mods/categories/54/).  
2. Install your armor mod and all prerequisite mods through Mod Organizer 2.
3. Install [Bethesda Launcher](https://bethesda.net/en/game/bethesda-launcher).
4. Launch Bethesda Launcher and install Creation Kit: Skyrim.
5. Edit your Windows Registry to allow Creation Kit to work with Skyrim VR.
	* Type "regedit" and hit ENTER in the Windows Search Bar > Navigate to HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Bethesda Softworks 
	* Right click on Bethesda Softworks and create a new Key called "Skyrim Special Edition" if it doesn't already exist.
	* Right click on "Skyrim Special Edition" and create a new String Value called "installed path" with the following value: C:\Program Files (x86)\Steam\steamapps\common\SkyrimVR\
6. Close the Registry Editor.
7. Uninstall and re-install Creation Kit from the Bethesda Launcher.
8. Open C:\Program Files (x86)\Steam\steamapps\common\SkyrimVR\CreationKit.ini and under the [General] section, add the following line: bAllowMultipleMasterLoads=1
9. Extract the contents of your armor mod using WinRAR or 7Zip.
10. Temporarily copy the .esp file from your armor mod to C:\Program Files (x86)\Steam\steamapps\common\SkyrimVR\Data  
11. Launch Bethesda.net Launcher >  Under Games, select Creation Kit: Skyrim and click PLAY.
12. Select File > Data... > Tick the plugin for your armor mod in the resulting window and click OK and YES.  Click "Yes to all" for any Warning messages.
13. Once the plugin is opened, click "Item" > "Armor" under the left hand bar in the Object Window.
14. Enter a snippet of the armor name for your mod in the "Filter" box in the upper left.
15. Under the "Name" field in the Object Window, note the names of EVERY piece of armor from your mod that you wish to use.
16. Close Creation Kit.
17. Delete the .esp file used in Step 9 from your Skyrim VR installation folder.
18. Launch Enderal VR.
19. When in-game, press "~" to open the console.
20. Type: help "ARMOR_NAME_FROM_CREATION_KIT" in quotations i.e. if Creation Kit listed an armor piece that you wanted called Necromancer Purple Boots, you would type: help "Necromancer Purple Boots" and hit ENTER.
21. The console will return the item code for the above item name.
22. Type: player.additem ITEM_CODE 1 i.e. player.additem 45010ADA 1
23. The armor associated with the item code will be added to your inventory.  Press "~" to exit the console.
24. Open your inventory, and you can now successfully equip the armor from your armor mod!  

## Supersampling
* For optimal image fidelity and performance, in-game Supersampling should always disabled.  Supersampling should always be performed using Contrast Adaptive Sharpening (CAS) via The Sharper Eye mod (pre-installed with this Wabbajack release).  To adjust The Sharper Eye values in-game, pressing the HOME key will open the built-in Reshade UI.  Here you can adjust the parameters for Contrast Adaptation, Max Color Delta, Sharpening Intensity, Contrast / Brightness / Color Saturation, and Sharpening Radius.  The END key will toggle the effects on or off, so you can use that to observe the difference the preset makes in the headset.  Default settings should be optimal for VR.  
* You can further optimize performance by installing [VR Performance Toolkit](https://github.com/fholger/vrperfkit/releases) to your Skyrim VR installation folder.
* In addition to improving visuals with The Sharper Eye, you can continue to supersample Enderal VR through SteamVR, the Oculus app, or Virtual Desktop.
    * If playing wired with an HTC/Valve/WMR headset, increase your SteamVR resolution above 100% to the maximum resolution your GPU can handle.  
    * If playing wired with an Oculus headset, increase your Render Resolution as high as your GPU can handle via the Oculus app.  
    * If playing wirelessly with Air Link, increase your Render Resolution as high as your GPU can handle via the Oculus app.  For optimal Air Link performance, set your Air Link Bitrate to around 50-100Mbps.  You can further optimize performance by installing [OpenComposite](https://gitlab.com/znixian/OpenOVR/) to your Skyrim VR installation folder.
    * If playing wirelessly with Virtual Desktop, lock your SteamVR resolution at 100% and set your Virtual Desktop video settings to Low/Medium/High based on your GPU. For optimal Virtual Desktop performance, set your Streaming settings to 60fps @ 80Mbps bitrate with Sliced Encoding enabled and SSW set to Auto.  You can also experiment with increasing the refresh rate to 90fps and toggling Video Buffering ON and OFF.  

# TAA
* Temporal Antialiasing (TAA) must always be active in Enderal VR or the in-game menu will exhibit visual glitches.  Unfortunately, TAA causes Enderal VR to look extremely blurry in-game and it also breaks parallax textures.  The best workaround for this problem is to leave TAA enabled while tweaking its settings to make its visual effects completely invisible in-game.  TAA settings cannot be configured via the main Skyrim VR INI files.  They must be configured using "VR FPS Stabilizer" under the [DataLoaded] section of the following INI file: \mods\VR FPS Stabilizer\SKSE\Plugins\VRFpsStabilizer.ini
* By default, this Wabbajack release leaves TAA enabled but tweaks the TAA effects to be completely invisible via VR FPS Stabilizer.  This enables parallax texture support but can also cause foliage flickering/pixelation.  If you wish to re-enable TAA effects, tick "Enable TAA FX" (or simply disable "VR FPS Stabilizer") in Mod Organizer 2.  Enabling TAA effects is NOT recommended as it will break parallax textures and cause visual glitches.

## Game capture
* If you want to take screenshots or record footage while in VR using an HTC/Valve/WMR headset, use [OBS Studio](https://obsproject.com) with the [OBS OpenVR Input Plugin v1.5](https://github.com/baffler/OBS-OpenVR-Input-Plugin/releases/tag/v1.5).  This will allow you to capture the game in widescreen at a higher resolution than what can be achieved when capturing the game from the SteamVR mirror window.

* If you want to take screenshots or record footage while in VR using an Oculus headset, use [OBS Studio](https://obsproject.com) with Oculus Mirror (found in C:\Program Files\Oculus\Support\oculus-diagnostics\OculusMirror.exe).  This is the best way to capture video from Skyrim VR due to the Oculus Mirror having a VR stabilizer to remove "shaky cam" effects from your recording.  To enable the VR stabilization feature, simply select Settings > Image Stabilization > Enabled.  For 1080p recording, create a shortcut to the Oculus Mirror with the following Target: "C:\Program Files\Oculus\Support\oculus-diagnostics\OculusMirror.exe" --Size 1920 1080.  To setup the recording process, launch Skyrim VR first through Link or Air Link.  Then launch Oculus Mirror and enable Image Stabilization.  Launch OBS Studio last and add a Window Capture source set to OculusMirror.exe.  For capturing audio, add an Audio Output Capture source set to Default.  

## Language packs
Enderal SE supports language packs which allow the game to be played in Chinese, French, German, Italian, Japanese, Korean, Russian, and Spanish.  You can download the packs [HERE](https://www.nexusmods.com/enderalspecialedition/mods/1?tab=files).  Install the language pack via Mod Organizer 2 with a unique name i.e. "Enderal SE - German Language Pack" and place it underneath "Enderal SE" and "Enderal SE - Update" in your mod loadout.  Finally, edit the following line "sLanguage=ENGLISH" with the preferred language in the following three files:
* C:\ (Your Game Folder)\mods\Enderal SE\Enderal - Forgotten Stories.ini
* C:\ (Your Game Folder)\mods\Enderal SE - Update\Enderal - Forgotten Stories.ini
* C:\ (Your Game Folder)\mods\Enderal VR\EnderalVRpatch.ini

If you are using a language pack, you may need to change the font used by Dear Diary or the menu interface may display incorrect characters.
- For French languages, select the Downloads tab in Mod Organizer 2.  Right click "Dear Diary VR - Paper SkyUI and Categorized Favorites-44874-1-06-1617397007.7z" and click "Install".  Select the following options:  Dear Diary VR > None > Rollover Menu Fix - MoreHUD VR > None > Tick "Sovngarde" > Click "Install" and "Replace".  This will update Dear Diary VR with the Sovngarde font which allows you to see French accented characters correctly.
- For languages using an extended Latin alphabet (with an umlaut mark or diaeresis) or the Cyrilic alphabet, select the Downloads tab in Mod Organizer 2.  Right click "Dear Diary-112-3-0-5-1624174013.zip" and click "Install".  Select the following options: Next > No > No > No > No/No > No/No > No > No > No > No > No > No > No > Yes (for "Install Tab Menu replacer") > No > No > No > No > Dark red quill (for "Replace the cursor?") > Select ENG (Latin) for the extended Latin alphabet or RU (Cyrilic) for the Cyrilic alphabet > None/No/No >  On the final page with the "Install" button, set the "Name" field to:  Dear Diary VR - Paper SkyUI and Categorized Favorites.  Then click "Install" and "Merge".  This will merge a new language font patch into Dear Diary VR.  

## Tools

[**Mod Organizer 2 v2.4.4**](https://www.nexusmods.com/skyrimspecialedition/mods/6194?tab=files): Mod Organizer (MO) is a tool for managing mod collections of arbitrary size. It is specifically designed for people who like to experiment with mods and thus need an easy and reliable way to install and uninstall them.

[**UI Tweaks v1.0**](https://www.nexusmods.com/skyrim/mods/70774/?tab=files): Theme for Mod Organizer, based on the default style with better and cleaner UI elements.

[**Nemesis Unlimited Behavior Engine v0.84-beta**](https://www.nexusmods.com/skyrimspecialedition/mods/60033?tab=files): An animation framework that enables behavior mods like CGO, SkySA, Ultimate Combat and most FNIS dependent mods to work together.

[**xLODGen Beta 97**](https://stepmodifications.org/forum/topic/13451-xlodgen-terrain-lod-beta-80-for-fnv-fo3-fo4-fo4vr-tes5-sse-tes5vr-enderal-enderalse/): Tool for generating terrain LOD.

[**DynDOLOD Standalone 3.0 Alpha-111**](https://www.nexusmods.com/skyrimspecialedition/mods/68518/?tab=files): DynDOLOD is a set of simple tools based on xEdit/xLODGen to automatically create a Skyrim mod based on the load order which adds distant LOD for objects and trees to Skyrim. By combining DynDOLOD with xLODGen users can create drastically enhanced static object LOD + tree LOD and the new, optional dynamic distant object LOD in a few simple steps.

[**Synthesis v0.25**](https://github.com/Mutagen-Modding/Synthesis): A framework and GUI to construct a single Bethesda game patch from many patcher sources. Designed to allow any program to work as a patcher as long as it conforms to the CLI API.

[**SSEEdit v4.0.4**](https://www.nexusmods.com/enderalspecialedition/mods/78?tab=files): SSEEdit is the Skyrim: Special Edition version of xEdit. xEdit is an advanced graphical module viewer/editor and conflict detector.

[**LOOT v0.18.6**](https://github.com/loot/loot/releases/): LOOT is a plugin load order optimisation tool for Skyrim VR.  It is designed to assist mod users in avoiding detrimental conflicts, by automatically calculating a load order that satisfies all plugin dependencies and maximises each plugin's impact on the user's game.

## Included Mods and Tools (Skyrim VR Installation Folder)
[**SKSE VR v2.0.12**](https://skse.silverlock.org): A tool used by many Skyrim mods that expands scripting capabilities and adds additional functionality to the game.

[**EngineFixesVR Part 2 v1.22**](https://www.nexusmods.com/skyrimspecialedition/mods/62089?tab=files): SKSEVR plugin to fix various issues with the Skyrim Special Edition engine.

[**d3dcompiler_47.dll**](https://www.nexusmods.com/skyrimspecialedition/mods/31963?tab=files): Install this to your Skyrim Special Edition folder if you don't already have a copy of d3dcompiler_47.dll

[**Binaural 3D Surround Sound for SKYRIM VR v2.3.01**](https://www.nexusmods.com/skyrimspecialedition/mods/26916?tab=files): This mod uses algorithms that can simulate HRTF, allowing for full 3D surround sound with just a normal pair of earphones or headphones. For 1st person use.

[**The Sharper Eye v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/46999/?tab=files): Get rid of the blur and grey mist in your headset which are clouding your vision. This VR-enabled ReShade build and preset provide the most performance-friendly sharpening filter for Skyrim VR bundled with a subtle touch of contrast, brightness and saturation. All configurable to your liking.
- Open "ReShadePreset.ini" and optionally set MaxDelta to 1.000000 to increase the sharpening effect.  Set to 0.070000 by default.

[**xSHADOWMANx's DLL Loader v1.0.0.4**](https://www.nexusmods.com/skyrimspecialedition/mods/3619?tab=files): DLL Loader for Dragonborn Speaks Naturally.

## Included Mods (Mod Organizer 2)
[**Enderal SE v2.0.8**](https://www.nexusmods.com/enderalspecialedition/mods/1?tab=files): Complete Enderal for Skyrim Special Edition.
- Add the following line to SKSE.ini (NPC Overhaul tweak):  iTintTextureResolution=2048

[**Enderal SE Update v2.0.8.2**](https://www.nexusmods.com/enderalspecialedition/mods/1?tab=files): Update for Complete Enderal for Skyrim Special Edition. 

[**Enderal SE Update v2.0.11**](https://eddoursul.win/mods/enderal-se/): Update for Complete Enderal for Skyrim Special Edition. 
- Remove "fs_se.dll"
- Do not update to Enderal SE v2.0.12 as it is not VR compatible.

[**Enderal SE - Bug Fixes v1.32**](https://www.nexusmods.com/enderalspecialedition/mods/2?tab=files): Removed the apparition script changes, which were slightly outdated. The fixes made by Bug Fixes are no longer needed.
- Do not install 2.0.12 update.

[**SkyUI v1.2.1**](https://github.com/Odie/skyui-vr): Elegant, PC-friendly interface mod with many advanced features.
- The new Highlight and Search features do not work if using "Dear Diary".

[**JContainers VR v4.1.13**](https://www.nexusmods.com/skyrimspecialedition/mods/16495?tab=files): Extends Skyrim SE Papyrus scripts (or SKSE/C++ plugins) with JSON based serializable data structures like arrays and maps. Embedded Lua interpreter.

[**moreHUD VR v1.1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/33215?tab=files): Adds more information to the HUD about the currently targeted object. Such as ingredients, weapon effects, potions, read books, v/w, enemy level, etc.

[**SkyrimVRTools v2.3-BETA**](https://www.nexusmods.com/skyrimspecialedition/mods/27782?tab=files): Providing OpenVR input information and control as a service to other Skyrim VR mods.

[**Enderal VR - Patch v3.3**](https://www.nexusmods.com/enderalspecialedition/mods/8?tab=files): Mod for playing Enderal in VR (with the SkyrimVR engine).

[**Enderal VR DynDOLOD Patch**]: Enderal VR ESP Fix for DynDOLOD 3.0 support.
- Removes all errors from FormID 00071C47 (ResourceObjectSawmill) in SkyrimVR.esm

[**SKSEVR 2.0.12**](https://skse.silverlock.org): A tool used by many Skyrim mods that expands scripting capabilities and adds additional functionality to the game.

[**EngineFixesVR v1.22a**](https://github.com/rollingrock/EngineFixesVR/releases): SKSEVR plugin to fix various issues with the Skyrim Special Edition engine.
- Open EngineFixesVR.ini and add the following lines: MemoryManager = false, SelectAllocator = 1.

[**VR Parallax Shader Fix v1.0.3**](https://www.nexusmods.com/skyrimspecialedition/mods/62090?tab=description): Injects fixed parallax shaders into Skyrim VR. Based on original code from aers under MIT.
- Requires Engine Fixes VR Part 2 in Skyrim folder
- Requires d3dcompiler_47.dll in Skyrim folder
- Required Load Order: SKSE, Engine Fixes VR, VR Parallax Shader Fix

[**VR Parallax Shader Fix - Experimental v1.0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/62090?tab=files): Injects fixed parallax shaders into Skyrim VR. Based on original code from aers under MIT. 
- Requires Engine Fixes VR Part 2 in Skyrim folder
- Requires d3dcompiler_47.dll in Skyrim folder
- Required Load Order: SKSE, Engine Fixes VR, VR Parallax Shader Fix, VR Parallax Shader Fix - Experimental

[**VR FPS Stabilizer v1.4.3**](https://www.nexusmods.com/skyrimspecialedition/mods/31392?tab=files): The VR FPS Stabilizer functionality of this mod is not being used with this Enderal VR release.  This mod has been included because it has the ability to automatically setup TAA (Temporal Anti-Aliasing) settings every time Enderal VR is launched.  TAA settings cannot be preconfigured with INI files and must be tweaked using VR FPS Stabilizer.  Default TAA settings will make Enderal VR look extremely blurry.  This can be quickly fixed by simply disabling TAA but this will also break Enderal VR menu artwork.  The best way to handle TAA is to tweak its settings with VR FPS Stabilizer to essentially disable all of its visual effects when enabled.  This allows Enderal VR menu artwork to work properly while keeping the visuals sharp without any blur in-game.  To remove TAA blur, add the following lines to \VR FPS Stabilizer\SKSE\Plugins\VRFpsStabilizer.ini:
- Do not use Location system or AutoConfig.
- GrassChange = 0 
-        taa sharp 2.285	 
         taa lf 0	 
         taa hf 0.8	 
         taa po 1.0	 
         taa ps 0

[**VR Address Library for SKSEVR v0.73**](https://www.nexusmods.com/skyrimspecialedition/mods/58101?tab=files): VR Address Library database for end users. This is intended as a VR replacement for Address Library for SKSE for mods designed for it. Only download if the mod says this is a requirement. It is currently an alpha. This is not for SSE. This is different from Address Library for SKSE.

[**Dynamic Animation Replacer for Skyrim VR 1415 v1.1.0a**](https://www.nexusmods.com/skyrimspecialedition/mods/33746?tab=files): This mod dynamically replaces the actors' animations depending on various conditions. Supports most actors, including creatures. Actors and animations added by mods are also supported. No ESP file.

[**Animation Motion Revolution VR v1.5.3**](https://www.nexusmods.com/skyrimspecialedition/mods/50258?tab=files): This SKSE plugin removes the mismatch between displacement and custom animations driven by motion data (the infamous ice-skating problem). Welcome to 2021 guys.

[**ADXP Beta v1.2**](https://www.skyrim-guild.com/distar/guidesandnews/mco-guide): A framework that bypasses the animation wall, allowing for modern combat in Skyrim.
- Delete MCO.dll

[**Crash Logger VR v1.7**](https://www.nexusmods.com/skyrimspecialedition/mods/59818?tab=files): Generates crash logs when the game Just Works™. This is a VR port using fudgyduff's MIT source.

[**PapyrusUtil VR - Scripting Utility Functions v3.6b**](https://www.nexusmods.com/skyrimspecialedition/mods/13048?tab=files): An SKSE plugin adding several new scripts with native functions that provide various conveniences related to data storage and other misc functions to the scripter/modder.  DynDOLOD requirement.

[**Papyrus Extender SSE v5.4**](https://www.nexusmods.com/skyrimspecialedition/mods/22854?tab=files): SKSE64 plugin that extends Papyrus script functionality, with over 275 new Papyrus functions, and 29 events.  
- Required by FEC.

[**Papyrus Extender VR v5.4**](https://www.nexusmods.com/skyrimspecialedition/mods/58296?tab=files): SKSEVR plugin that extends Papyrus script functionality, with over 275 new Papyrus functions, and 29 events. This requires the original Papyrus Extender and is built from po3's source.
- Required by FEC.

[**DynDOLOD Resources SE v3.00 Alpha-30**](https://www.nexusmods.com/skyrimspecialedition/mods/52897?tab=files): DynDOLOD is a set of simple tools based on xEdit/xLODGen to automatically create a Skyrim mod based on the load order which adds distant LOD for objects and trees to Skyrim. By combining DynDOLOD with xLODGen users can create drastically enhanced static object LOD + tree LOD and the new, optional dynamic distant object LOD in a few simple steps.

[**More Informative Console VR v1.1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/19250?tab=files): This mod edits the UI to show a great deal of additional information on npcs, items, and other objects when the console is opened, similar to the way MFG console worked for Oldrim.

[**Dear Diary VR - Paper SkyUI and Categorized Favorites v1.06**](https://www.nexusmods.com/skyrimspecialedition/mods/44874?tab=files): Replacer for Skyrim interface in a paper style.

[**Dear Diary - Paper UI Replacer for Enderal SE v3.0.5**](https://www.nexusmods.com/enderalspecialedition/mods/112?tab=files):  Updates Dear Diary for Enderal compatibility.  Removes "Skills" option from the Tab Menu as this menu is not used by Enderal and will cause the game to crash when accessed if not removed.
- Install Tab Menu ONLY.

[**VR Menu Mouse Fix v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/33414?tab=files): Enables mouse for SkyUI-VR. You can use your controllers to control the cursor like a smart tv remote.

[**Smaller HUD for VR v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/30726?tab=files): A simple mod that reduces the size of the HUD elements by about 50%.

[**Dot Crosshair VR v0.8**](https://www.nexusmods.com/skyrimspecialedition/mods/17764?tab=files): Colors the target crosshairs as red and green and converts them to dots since the default grey target crosshairs are often difficult to see and you can not distinguish them in casting double magic.

[**RaceMenu SE v0.4.19.11**](https://www.nexusmods.com/skyrimspecialedition/mods/19080?tab=files): Complete overhaul to the character creation menu including new customization features such as multiple RGBA warpaints, body paints, hand paint, and foot paints.
- Remove skee64.dll an skee64.ini

[**RaceMenu VR v0.4.14**](https://www.nexusmods.com/skyrimspecialedition/mods/19080?tab=files): VR patch for RaceMenu.

[**Smaller HUD for VR Larger Text Patch**]: An override patch for [Smaller HUD for VR](https://www.nexusmods.com/skyrimspecialedition/mods/30726?tab=files) to increase text size while retaining the smaller HUD elements from the original mod.  Overrides "Smaller HUD for VR" with vanilla skyvr_hmd_info.nif to increase text size.  Rescales Health, Magica, Stamina, and Quest Update Base Instance sprites in vr_hmd_info.swf to shrink HUD elements from vanilla Skyrim back to the smaller sizes used in the original "Smaller HUD for VR" mod.  Shifts Quest Update Base Instance sprite on X-axis to prevent menu clipping.  Patch created with JPEXS Free Flash Decompiler.
- Place after other Skyrim SE HUD mods.

[**Path of the Prophet (No Floating Quest Marker) v1.01**](https://www.nexusmods.com/skyrimspecialedition/mods/63279): Removes floating quest markers from the game.  Quest markers are still viewable on the compass.

[**MCM Recorder v1.07**](https://www.nexusmods.com/skyrimspecialedition/mods/61719?tab=files): Configuring MCMs has never been easier!
- Place JSON scripts in \McmRecorder\Recording_XXX_XXXXXX\ folder 
- Edit JSON scripts and set "autorun": "true"

[**Nemesis Unlimited Behavior Engine v0.84-beta**](https://www.nexusmods.com/skyrimspecialedition/mods/60033?tab=files): An animation framework that enables behavior mods like CGO, SkySA, Ultimate Combat and most FNIS dependent mods to work together.

[**Spell Perk Item Distributor VR v6.3.0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/59121?tab=files): SKSEVR plugin that can be used to add spells/perks/items/shouts/packages/outfits/keywords/factions to every NPC in the game, using config files. This is the VR version built from po3's source.

[**Base Object Swapper VR v2.5.1**](https://www.nexusmods.com/skyrimspecialedition/mods/61734?tab=files): SKSE plugin and framework for swapping base objects and references, using config files. VR port of MIT source.

[**VRIK V0.8.1. In-Dev Build 28**](https://www.nexusmods.com/skyrimspecialedition/mods/23416?tab=files): VRIK will display the player character's body in SkyrimVR and animate it to match your movements. Weapons can be kept, drawn, and sheathed in up to 14 visible holsters on your body. An input gesture system allows users to bind actions to gestures on each hand, reducing the need to open menus. An MCM menu allows full configuration of everything.
- Make the following changes to these VRIK INI files to pre-configure MCM settings with proper behavior for bows:  
	- vrik.ini: weaponAdjustment = 0
	- vrikslots.ini: visibleSlot11 = 0 
- Make the following changes to these VRIK INI files to pre-configure MCM settings for Selfie Mode:  
	- vrikgestures.ini: selfieModeEnabled = 1
- Make the following changes to these VRIK INI files to pre-configure MCM settings to allow for open hand spell casting:  
	- vrikgestures.ini: castWhenHandsOpen = 2

[**Arctal's VRIK Tweaks v1.5**](https://www.nexusmods.com/skyrimspecialedition/mods/63663?tab=files): Fixes some pet peeves of mine with the VRIK mod. Currently including gesture system improvements, changes to ragdolling during knockback/death and a near-clip-distance bug fix.

[**VRIK Neardistance Fix Patch for Build**]: Sets fNearDistance to 13 to fix mountain flickering.

[**HIGGS - Enhanced VR Interaction v1.5.10**](https://www.nexusmods.com/skyrimspecialedition/mods/43930?tab=files): Hand/weapon collision, realistic object grabbing, and gravity gloves-style mechanics for Skyrim VR.
- Remove any [HAVOK] settings from your Skyrim INI files as these settings are no longer necessary with HIGGS VR v1.2+.
- Make the following changes to higgs_vr.ini to make all held objects use velocity-based movement (recommended):
	- ForcePhysicsGrab = 1

[**PLANCK v0.5**](https://www.nexusmods.com/skyrimspecialedition/mods/66025?tab=files): Physically-driven animation in Skyrim. Characters interact with physics and can be grabbed, melee hit detection is physically accurate, and much more.

[**Spell Wheel VR v1.3.0**](https://www.nexusmods.com/skyrimspecialedition/mods/47630?tab=files): Selection wheel mod for Skyrim VR. It allows you to select spells, weapons, shields, arrows, potions, poisons, food, torch, armors and more without going into a menu very quickly by press of a button or button combinations to spawn the wheel and hold your hand over the item and letting go of the button. It's equipped automatically.

[**Enchanted Weapons Charge Fix v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/62314?tab=files): Ever wondered why your enchanted weapon not charging when using Soul Siphon perk from Ordinator? Or why Summermyst's enchanted glove not recharging your weapon past the initial value when equipped? It's because there's a bug in Skyrim engine that prevent you from doing so. This mod will fix that and allow weapons to charge to their maximum limit.
- Do not update to v2.0 as the lastest version is not VR compatible.

[**Wearable Health Bars - Soul Gauge v1.6**](https://www.nexusmods.com/skyrimspecialedition/mods/65737?tab=files): Jewelry that displays Health, Magicka, Stamina, enchantment charge, or equipped ammo count on your hands. Glows in the dark!

[**Spellsiphon - Complete Edition v5.23**](https://www.nexusmods.com/enderalspecialedition/mods/357?tab=files): Experience gameplay focused on combos and synergy. Lessen the need for menus or hotkeys through a system where swapping spells and weapons is streamlined and rewarding. Continue the fight at 0 magicka by using new spell types. Enjoy a plethora of new sounds and visual effects. Grow in power by playing skillfully, not just from levels and gear.

[**Magic Improvements for Skyrim VR v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/55751?tab=files): Vastly improved dual casting, spell effect size scales based on magicka percentage, and additional options for aiming spells in VR.

[**Improved Bound Sword and Dagger Collision v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/60064?tab=files): More accurate collision for the bound dagger and sword.

[**NavigateVR v1.51**](https://www.nexusmods.com/skyrimspecialedition/mods/47174?tab=files): This mod brings immersive navigation to VR with a functional compass.
- Replace "LHandTamrielSettlements.dds" and "RHandTamrielSettlements.dds" with maps of your choice from the "Maps - SE" or "Anna's Enderal Map" mod to make the default Navigate VR map artwork lore friendly to Enderal.
- Remove "Map of Skyrim" and "Map Storage Case" from the plugin's "Misc. Item" data along with "FormID List".startingitems and under Weapon.TRC_WorldMap, Quest.TRC_MapQuest set '110C0BBC' and '1110CC1D' records to 0, and under Quest.TRC_MaintenanceQuest remove the '110C0BBC' and '1110CC1D' records using xEdit to completely remove the broken map from the mod. 
- Rename "Map of Provinces and Isles" to "Map of Enderal" from Weapon."Map of Provinces and Isles".OBND."FULL - Name" in xEdit to give the NavigateVR map a lore friendly name.

[**Splashes of Skyrim - VR v1.2.1**](https://www.nexusmods.com/skyrimspecialedition/mods/47710?tab=files): SKSE plugin that adds projectile based water splashes and ripples, and underwater explosions.

[**Splashes of Storms v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/72115?tab=files): SKSE plugin that adds splashes and ripples when raining.

[**Splashes of Storms VR v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/73111?tab=files): SKSE plugin that adds projectile based water splashes and ripples, and underwater explosions.

[**DragonbornSpeaksNaturally - Beta v0.21.1-beta**](https://www.nexusmods.com/skyrimspecialedition/mods/16514?tab=files): Adds speech recognition to Skyrim VR or Skyrim SE so you can recite your dialogue lines to select them.

[**Immersive Gathering (Woodchopping and Mining) SE - VR Friendly v1.7**](https://www.nexusmods.com/skyrimspecialedition/mods/29710?tab=files): Chop wood and mine ore for real!

[**Destructible Bottles Extended v1.5**](https://www.nexusmods.com/skyrim/mods/26017?tab=files): Hit the bottle and smash it in pieces! Latest version 1.5 includes also some glazed pottery items such as pots, jugs, plates and bowls.
- LE mod.  Converted to Form 44 (SE) by opening and resaving ESP file in Creation Kit.
- Needs processed by Cathedral Assets Optimizer with the following settings enabled: Process meshes, Full optimization, Always process headparts, Resave meshes. Process textures, necessary optimization, Compress textures, Generate mipmaps.  

[**Alternative Smashing Glass Sounds v1.0**](https://www.nexusmods.com/skyrim/mods/26017?tab=files): Alternative HQ glass sounds thanks to rolloLG.

[**Destructible Skyrim - Base Object Swapper v0.5.3.1**](https://www.nexusmods.com/skyrimspecialedition/mods/77568?tab=files): Smash, shout, and blow up the environment around you, without the need for silly, complicated patches! Be careful, though - just like with stealing, people aren't very fond of the destruction of their property!
- Remove "Moveable Static" records in xEdit to fix invisible lanterns.

[**Immersive Decomposing Dead v0.1.5**](https://www.nexusmods.com/skyrimspecialedition/mods/66166?tab=files): This mod makes it so dead bodies (NPCS and animals) decompose until turned into bones (a prosses that might attract rats). Also makes it so the dead are buried fast by npcs in a few towns.

[**Moons and Stars - Sky Overhaul SKSE v2.0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/73336?tab=files): DLL plugin to fix moons and stars movement and phases.

[**Moons and Stars - Sky Overhaul SKSEVR v2.0**](https://www.nexusmods.com/skyrimspecialedition/mods/73667?tab=files): DLL plugin to fix moons and stars movement and phases. VR port using po3's MIT source code.

[**Immersive Smithing v1.0.4**](https://www.nexusmods.com/skyrimspecialedition/mods/72298): It's time to "be the smith".... With the help of VRIK, Spell Wheel & HIGGS and with your trusty Black Smiths hammer in hand, improve weapons and armor like never before!

[**ElSopa - HD Grindstone Redone SE Patch v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/72298): Add compatibility for ElSopa's 'HD Grindstone Redone SE' mod. Place below the original mod in your load order and overwrite any files if required. Thanks to ElSopa for permission to use his meshes for this patch.

[**ElSopa - HD Medieval Anvil SE Patch v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/72298): Adds compatibility for 'ElSopa - HD Medieval Anvil SE' Mod. Place this patch below the original in your load order and overwrite any files. Thanks to ElSopa for the permissions to use his meshes.

[**HapticSkyrimVR - Spellcasting and Enhanced Bow and Melee Feedback SKSE Plugin v1.7.2**](https://www.nexusmods.com/skyrimspecialedition/mods/20364?tab=files): SKSEVR plugin to get spell casting and enhanced bow and melee haptic feedback on VR controllers.

[**Simple Realistic Archery VR v1.26**](https://www.nexusmods.com/skyrimspecialedition/mods/28524?tab=files): Automatically unequips your arrows after shooting them, then reequips the arrow after pressing the trigger (MCM configurable) over your shoulder. It also has options for binding different arrows to different buttons, for the position and size of the quiver, and options for attribute costs. Up to 25 arrow types can be bound at once.

[**Weapon Throw VR v1.3.5**](https://www.nexusmods.com/skyrimspecialedition/mods/31374?tab=files): Allows you to throw your equipped weapons in VR by holding a button, swinging your hand, and releasing it. All six melee weapon types, shields and torches are supported. Supports vanilla and mod added weapons. Includes Auto-Return and Auto-Aim features. Comes with an MCM to configure every setting.

[**Dual Wield Block VR v1.7**](https://www.nexusmods.com/skyrimspecialedition/mods/28456?tab=files): SKSE plugin to let the player block attacks while dual wielding (two weapons or weapon + spell) or unarmed.

[**LocationalDamageSKSE VR v0.7.2**](https://www.nexusmods.com/skyrimspecialedition/mods/26447?tab=files): Locational Damage for SKSE VR! Do extra damage depending on which body part you hit with your arrows or spells.

[**No Stagger Mod v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/16335?tab=files): This mod makes your character unstaggerable. 

[**Sprint Jump VR v1.1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/28354?tab=files): An SKSE plugin to allow Sprint Jumping in SkyrimVR. Increase sprint jump height and distance with a multiplier in the config file.

[**Enhanced Ragdoll Accuracy Main File v1.02**](https://www.nexusmods.com/skyrimspecialedition/mods/45767?tab=files): Makes in-game humanoid corpses much more believable and immersive through meticulous changes in weight, joints, etc.

[**Scoped Bows SE v1.3.1**](https://www.nexusmods.com/skyrimspecialedition/mods/912?tab=files): Scoped Bows is a huge weapons mod that adds scoped variants of all bows to the game, designed to be used without crosshair.
- "Cell" and "Worldspace" data must be removed from ScopedBows.esp using xEdit or DynDOLOD 3.0 will fail.

[**Scoped VR-1-1-1 v1.1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/16666?tab=files): Scoped Bows Remixed meshes designed for VR.

[**Sighted Crossbows VR v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/28948?tab=files): Sights for Crossbows Skyrim VR.

[**Simple Iron Sights for Sighted Crossbows VR v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/38946?tab=files): Changes the sights included in Sighted Crossbows VR into more of a simplistic, medieval style.

[**Instant Equip v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/44571?tab=files): SKSE plugin that essentially skips weapon drawing and sheathing animations.

[**Immersive Draw Sheathe Sounds v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/44992?tab=files): This improves the Draw/Sheathe sounds for use in VR.

[**Blocking and Flash VR - Block Sparks and Impact Sounds v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/74463): Block Sparks & Impact Sounds for Skyrim VR without affecting gameplay.

[**SMIM v2.08**](https://www.nexusmods.com/skyrimspecialedition/mods/659?tab=files): A massive project to greatly improve the appearance of countless static 3D models in Skyrim. Basically, this is my attempt to make the Skyrim architecture, clutter, furniture, and landscaping much nicer.
- Place above all other texture/mesh mods to avoid SMIM conflicts.
- Remove \meshes\architecture\farmhouse\farmhousewindmill, \meshes\architecture\solitude\swindmill.nif, and \meshes\architecture\solitude\swindmillrotor.nif to revert windmills back to vanilla which arguably look better in VR.
- Remove ESP file.

[**SMIM Compatible Smelter v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/72298): Overwrite SMIM smelter with this file.

[**Enderal Texture Workshop v1.5**](https://www.nexusmods.com/enderal/mods/275?tab=files): Vanilla-friendly retexture for various assets in Enderal.
- Recommend installing before Enderal SE Retexture Pack Project.

[**Noble Skyrim FULL PACK Performance Edition v5.5.0**](https://www.nexusmods.com/skyrimspecialedition/mods/21423?tab=files): Gives all of Skyrim's architecture a complete new look by changing its textures to custom ones. Beside the architecture, several other things, such as landscape, dungeons (ruins, mines, caves etc.), clutter stuff etc. have been re-textured as well, to match the rest of the mod.
- Recommend placing before other Skyrim texture packs; Remove "whroughgroundmud.dds".

[**Solitude HD by CleverCharff 4K 2K v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/33885?tab=files): Retexture of Solitude assets both interior and exterior. Available in 4K and 2K.

[**Enderal SE Retexture Pack Project - Architecture Medium Quality v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/407?tab=files): A port of my Special Edition texture mod (SNRP) featuring edited textures as well as new to fit the aesthetics of Enderal. Still a work in progress.
- Remove \meshes\ folder

[**Enderal SE Retexture Pack Project - Dungeons Medium Quality v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/407?tab=files): A port of my Special Edition texture mod (SNRP) featuring edited textures as well as new to fit the aesthetics of Enderal. Still a work in progress.
- Remove \meshes\ folder

[**Enderal SE Retexture Pack Project - Landscapes and Trees Medium Quality v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/407?tab=files): A port of my Special Edition texture mod (SNRP) featuring edited textures as well as new to fit the aesthetics of Enderal. Still a work in progress.

[**Enderal SE Retexture Pack Project - Ruins and Misc Medium Quality v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/407?tab=files): A port of my Special Edition texture mod (SNRP) featuring edited textures as well as new to fit the aesthetics of Enderal. Still a work in progress.
- Remove \meshes\ folder

[**Enderal SE Retexture Pack Project - Ruins and Misc Medium Quality v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/407?tab=files): A port of my Special Edition texture mod (SNRP) featuring edited textures as well as new to fit the aesthetics of Enderal. Still a work in progress.
- Remove \meshes\ folder

[**Noble Skyrim Dwemer Ruin Textures Performance Edition v5.5.0**](https://www.nexusmods.com/skyrimspecialedition/mods/21423?tab=files): Gives all of Skyrim's architecture a complete new look by changing its textures to custom ones. Beside the architecture, several other things, such as landscape, dungeons (ruins, mines, caves etc.), clutter stuff etc. have been re-textured as well, to match the rest of the mod.
- If using Enderal SE Retexture Pack Project, recommend overriding the mod with Noble Dwemer Ruin textures.

[**Tamrielic Textures SE 1 Landscapes 1K v1.4.0**](https://www.nexusmods.com/skyrimspecialedition/mods/32973?tab=files):  A fresh and complete replacement of all Skyrim landscape textures.

[**Septentrional Landscapes SE - 2K v1.3.2**](https://www.nexusmods.com/skyrimspecialedition/mods/29842?tab=files): Landscape textures made with 3D Scans. 8, 4 & 2K versions available.

[**4K SMIM Whiterun Bench v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/32164?tab=files): Retextures the SMIM bench in Whiterun with darker and dirtier options available.

[**4K SMIM Furniture Improvement v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/32552?tab=files): A 4K retexture of SMIM furniture textures.

[**4K SMIM Furniture Chest v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/33369?tab=files): A retexture of the SMIM furniture chests, Upperclass, Weathered, Open and Snow. 4K or 2K.

[**SMIM Food Resized - All In One v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/72797?tab=files): A size reduction of the SMIM food models for VR and SSE.

[**Silver Objects SMIMed v.4**](https://www.nexusmods.com/skyrimspecialedition/mods/70787?tab=files): Improve silver objects 3D models and shaders. Affects silver, Sovngarde, common, and Thieves Guild quest items.

[**Venerable Nordic Temples (2K - 4K) v0.2**](https://www.nexusmods.com/skyrimspecialedition/mods/38544?tab=files): A high quality retexture for Nordic temples and ruins, offering high fidelity visuals and a lore friendly, ancient aesthetic.

[**Underground - A Dungeon Texture Overhaul v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/14365?tab=files): An ambitious dungeon retexturing project which starts with caves and Nordic dungeons.
- Place high on load order so mod is overwritten by other texture mods.
- Noble Skyrim has vastly superior Dwemer textures versus Underground.  If using Noble Skyrim, it is recommended to place the Underground mod UNDER Noble Skyrim.  Then navigate to \Underground - a dungeon texture overhaul\textures\dungeons\dwemerruins\ and remove ALL files with the exception of dwestonefloor**.*  This will ensure that Noble Skyrim's superior Dwemer Ruins textures will take precedence over Underground.

[**Misc Retexture Project v2.7**](https://www.nexusmods.com/skyrimspecialedition/mods/13578?tab=files): An ongoing project to find and retexture overlooked items throughout Skyrim.

[**MRP 2.6 Small Update v2.6.2**](https://www.nexusmods.com/skyrimspecialedition/mods/13578?tab=files): A small update, added the fox and wolf pelts and also the chicken.

[**Rustic Clutter Collection - SE - 2K v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/5795?tab=files): This is a collection of my Rustic clutter item retextures. The mod includes RUSTIC DINNERWARE, RUSTIC POTTERY, and RUSTIC SILVERWARE. There are also a few other clutter items like mead bottles, wine bottles, the satchel, knapsack, coin purse, strongbox, safe, prisoner cage, and the dwemer lexicon cubes. 2K and 1K versions available. 

[**Realistic HD Mods Remastered Collection - 2K v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/5795?tab=files): Collection of all Remastered Realistic HD Series Mods for SSE (All in One).  

[**Better Wine Labels - Vanilla v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/34698?tab=files): HD wine label textures for the vanilla wine label and ones added by Legacy of the Dragonborn.

[**Better Wine Labels - San's Spiced Wine  v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/34698?tab=files): 2x size and cleaner than vanilla but not that much of an improvement (the label is very small in-game). Can be used with either of the main files.

[**Pretty Animated Potions - VR Edition v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/52663?tab=files): Yet another animated potions mod. This time in small bottles! 1K retexture. Refracting bottles option available!

[**JS Purses and Septims SE v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/37306?tab=files): A complete re-creation of Septims, Coin Purses and Coin Piles.

[**VR Refit - JS Purses and Septims Resized v1.0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/49850?tab=files): A VR mod for smaller coins, coin purses, and coin piles from JS Purses and Septims. It also patches the invisible coin purse drop sound bug.

[**Rally's Candlelight and Magelight Fix SE - VR v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/36594?tab=files): Fix for the Candlelight Spell and Magelight Spell in SE/VR.

[**JS Instruments of Skyrim SE v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/51959?tab=files): A complete remake of the Lute, Flute & Drum. Comes in 2k and 4k versions.
- Delete ESP file.

[**Real Mountains Rebuilt v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/3704?tab=files): Retexture that enhance the detail of mountains and rocks.

[**WiZkiD Carriages v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/39640?tab=files): A complete replacer for all carriages with high quality textures.

[**WiZkiD Parallax Farmhouses 2k No Parallax v1.4**](https://www.nexusmods.com/skyrimspecialedition/mods/39185?tab=files): A complete overhaul of all farmhouses related models with high quality textures. This overhaul includes exteriors, interiors, basement and stonewalls.
- If using Enderal SE Retexture Pack Project, recommend removing \meshes\architecture\farmhouse\farmwell01.nif

[**ElSopa - HD Grindstone Redone SE 1K v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/58149?tab=files): Grindstone Redone. New Mesh. New Textures. No ESP. Optional Texture Resolutions.

[**El Sopa - HD Medieval Anvil SE v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/48825?tab=files): New Model And Textures For The Anvil . The Hammer And Tongs. Performance Friendly. Ultra Immersive. All Resolutions. No ESP.
- Delete blacksmithnovicetongs01.nif (this mesh causes visual glitches).

[**Inferno - Fire Effects Redux v5.1**](https://www.nexusmods.com/skyrimspecialedition/mods/29316?tab=files): Spiritual successor to the original Ultimate HD Fire Effects mod by rheadude with improved meshes and textures! 
- Use the following installation options: No ENB Light > 4x > Normal > Realistic Hue > 1x > Vanilla > No Plugin
- ESP file not supported.  Do not install patches.
- Remove \meshes\weapons\torch.nif to fix blue torch flames.

[**Embers XD v2.6.9**](https://www.nexusmods.com/skyrimspecialedition/mods/37085?tab=files): An overhaul of campfires and other fire sources.
- Use "Inferno Flames" if using "Inferno - Fire Effects Redux".
- Install Forges and Lava Craters Add-On.
- Delete ESP files.

[**Embers XD - Living Temple CTD Fix v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/421?tab=files): Replaces "giantcampfire01off.nif" back to vanilla mesh to avoid CTD when entering Living Temple.

[**Animated Forge Water v0.6**](https://www.nexusmods.com/skyrimspecialedition/mods/52322?tab=files): A mesh only animated forge water replacer with refraction. No ESP. Includes patches for Elsopa and Embers.
- Install "Elsopa and Embers XD" patch. 

[**HLP Night Sky High v2.07**](https://www.nexusmods.com/skyrimspecialedition/mods/8752?tab=files): HLP Night Sky offers a tasteful, realistic, and lore-friendly replacement of the night sky textures (stars, constellations, and the milky way. 

[**STO - Stars 4K Only small stars v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/4931?tab=files): Overhauls the stars to 4K from 1K. Adds some big stars but most is small stars you can also chose to have only small stars, Glimmers dynamically when moving around.

[**RIS - Real Ice and Snow v2.5.1**](https://www.nexusmods.com/skyrimspecialedition/mods/1484?tab=files): ONE OF THE BEST SNOW MODS FOR OLDRIM, FINALLY IN SSE WITH UPDATED MESHES AND TEXTURES! Snow that looks like real snow. Icicles that look like real icicles. Icebergs that look like real icebergs. Icefloes that look like real icefloes.

[**Fluffy Snow v1.4**](https://www.nexusmods.com/skyrimspecialedition/mods/8955?tab=files): Simple texture replacer for snow. The aim is to make the snow a little more fluffy than vanilla.

[**HD Transparent Smaller Snowflakes 2K v1.0**](https://www.nexusmods.com/skyrim/mods/74048?tab=files): This mod replaces the default Skyrim snowflakes with Ultra HD Ultra Realistic Transparent Crystal Snowflakes. 
- Needs processed by Cathedral Assets Optimizer with the following settings enabled: Process meshes, Full optimization, Always process headparts, Resave meshes. Process textures, necessary optimization, Compress textures, Generate mipmaps.  

[**Remove Blurry Snowflakes v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/38358?tab=files): This mod removes the blurry snowflakes by using a transparent texture. The normal snowflakes are still present.

[**Glorious Doors of Skyrim v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/32376?tab=files): All-In-One pack of all my doors including a handy Fomod installer and a new Dwemer door!
- Delete ESP file.

[**Vanilla Table Replacers v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/33041?tab=files): Replaces some tables of the game specially the main tables for nobles.

[**DUST x2048 By Ramccoid v6.1**](https://www.nexusmods.com/skyrimspecialedition/mods/38444?tab=files): This mod retextures the ambient dust particles which float in the air and also the falling dust effect in dungeons and such places.

[**Kanjs - Chaurus eggs and staff v2.1**](https://www.nexusmods.com/skyrimspecialedition/mods/46486?tab=files): A Simple Chaurus Egss Meshes and Textures remade ! With an optional Staff!
- ESP file not supported.  Select "No Staff" options which use no plugins.

[**3D Casting FX - Fire and Frost Hand FX Replacer v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/50197?tab=files): Replaces the effect in your hand when holding a fire or frost spell. The vanilla effects are made up of 2D sprites moving in a single plane which is very apparent and quite ugly in VR. These new ones are specifically designed to look good in VR and SE both.

[**Loose Clear refracting icicle and FrostAtronach v1.5**](https://www.nexusmods.com/skyrimspecialedition/mods/2458?tab=files): Realistic looking Icicle and Frost Atronach.

[**Rallys City Roofs 2K - AIO v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/20896?tab=files): This mod retextures the roofs of houses and market stalls in Whiterun, Riften and Solitude.
- If using Enderal SE Retexture Pack Project, recommend removing wrmarketstallroof01*.*

[**Rally's Mead Barrels v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/49641?tab=files): Replacer for mead barrels and spigots.

[**Renthal's Workbench v1.4**](https://www.nexusmods.com/skyrimspecialedition/mods/23164?tab=files): New high poly mesh and texture for the workbench.

[**Better Dirt Cliffs and Alphas v4.0**](https://www.nexusmods.com/skyrimspecialedition/mods/34035?tab=files): Overhaul of the meshes & alpha channels involved in blending the top of the dirt cliff with the roots, and the roots with the wall. Covers SMIM meshes too.

[**Enhanced Vanilla Trees SE-Lush Trees v2.2.1**](https://www.nexusmods.com/skyrimspecialedition/mods/11008?tab=files): Better Vanilla Trees? Sign me up! All-In-One tree overhaul package with enhanced Vanilla trees. Supports RAT, SFO Branches, SFO Snowy Pines, and more!
- Recommend installing with Vanilla (i.e., None), Realistic Aspen Trees, SFO Snowy Pine Trees with all other settings left at default.
- Keep \DYNDOLOD\ folders.  Used by DynDOLOD 3.
- Remove the plugin's "Worldspace" data in xEdit.
- After running DynDOLOD 3... 1) Optionally delete ESP file to save a plugin slot.  2) Navigate to \Enhanced Vanilla Trees SE-Lush Trees\meshes\landscape\trees\ and remove SRG_ prefix from filenames.  Required if not using plugin.

[**HD Dead Trees and Driftwoods v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/35308?tab=files): Combine "4K Parallax Treebark" and "Spooknik's - Tundra Trees HD" to achieve HD dead trees and driftwoods. Contains original mods port.

[**CC's Enhanced Ore Veins SSE Edition v9.0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/1306?tab=files): A texture replacement for the ore veins found in mines and around skyrim. This mod also retextures the mined ores and the ingots.

[**Rustic Alchemy and Enchanting Tables v1.0**](https://www.nexusmods.com/skyrim/mods/62328?tab=files): A rustic overhaul of the alchemy and enchanting tables of Skyrim. The aim was to bring real antiquity to these arcane crafting tables as is fitting of their ancient origin.

[**WEBS v0.2**](https://www.nexusmods.com/skyrim/mods/33718?tab=files): A complete set of 1k texture replacers for the default webs and cobwebs. 

[**Snazzy Furniture and Clutter Overhaul SE v2.1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/2414?tab=files): Comprehensive overhaul of furniture and clutter throughout Tamriel, including: - New HD noble chairs, beds, drapery, Imperial Banners, etc. - Several styles of weapon racks, plaques, and display cases - Many new wall art paintings.
- ESP file not supported.  Install "Replacer Version" which uses no plugins.

[**Jabber's 2K Archery Targets v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/21726?tab=files): Retextures the SMIM archery targets with high-quality 2K textures.

[**Training Dummies Retexture 4K v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/13522?tab=files): Replaces vanilla training dummies. 2k and 4k Versions. This mod was requested by several people. So here it is! No esp needed. Just a texture replacer.

[**Realistic Paper Parchment v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/44223?tab=files): Couldn't find a good texture so I've made one.

[**Realistic Paper Scrolls v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/44223?tab=files): Couldn't find a good texture so I've made one.

[**Pillows - My HD Version SE v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/43752?tab=files): HD replace for the pillows of all the beds. Adds missing pillows, like to the orcish beds. HD noble beds texture (4K).

[**4K Bedroll v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/46101?tab=files): Simple texture replacer for the bedroll and an alt texture if you want it.  4K textures.

[**Boreal Boats SE - 4K v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/47608?tab=files): A ship and Boat retexture in 8, 4 or 2K, with parallax enabled meshes. The roof now has its own texture with environment mapping, no more sharing textures with whiterun. Ships with optional closed roof version in 8-2K resolution.

[**ElSopa - High Quality Buckets SE v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/47227?tab=files): High Quality Buckets. New Meshes And Textures. All Resolutions. No ESP.

[**ElSopa - High Quality Buckets SE - HOTFIX v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/47227?tab=files): Missing Meshes.

[**Skyrim Posts Replacer v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/29625?tab=files): Replaces most of the posts in skyrim and i made it close to the original as possible because I don't want to completely change the original model.

[**Tihzz's Lantern HD Replacer 4K v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/25361?tab=files): A simple model replacement for the candlelanternwithcandle01 and candlelantern01.

[**Cinematic Light Sprite (Candles and Lanterns) v1.0**](https://www.nexusmods.com/skyrim/mods/78160?tab=files): Replace candles and lantern lightsprite.

[**Organic Riften Leaves 2K v1.02**](https://www.nexusmods.com/skyrimspecialedition/mods/17911?tab=files): Quality textures for the fallen leaves in Riften 4K, 2K, 1K.

[**Dwemer Pipework Reworked v4.0**](https://www.nexusmods.com/skyrimspecialedition/mods/46507?tab=files): Rework of Dwemer pipes, including Dwemer boilers.

[**Stockade Old Grey Timber 4k New-1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/15501?tab=files): A 4k or 2k retexturing of all stockade wood textures. These are found at farms, in forts, and out the front of mines Three options are now available due to popular request: Old Grey, Painted and Brown!

[**Nightingale Pride 4K SSE Edition - With Gems v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/22813?tab=files): High Resolution, Lore Friendly Retexture Of Nightingales Bow and Blade. Polished for SSE EDITION.

[**Auriels Holy Bow 4K - REDUX v4.0**](https://www.nexusmods.com/skyrimspecialedition/mods/2069?tab=files): I am proud to present a totally remade version of my Auriel's Holy bow mod for Skyrim Special Edition. This mod adds a really cool looking glow to the Auriel's Bow from the Dawnguard DLC.
- Delete ESP file.

[**Advanced Alloys Carbon Fiber Reinforced Dwarven Crossbow v1.0**](https://www.nexusmods.com/skyrim/mods/23646?tab=files): Texture replacer for Dwemer crossbow.

[**1K Farmhouse Fences SE Version 2 v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/38912?tab=files): Two new fences for Skyrim farmhouse wovenfences available in 4k, 2k and 1k.

[**Skyrim Textures Redone - High Hrothgar 2K v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/13621?tab=files): Complete texture overhaul for High Hrothgar, Offers studio quality baked normals and baked ambient occlusion maps with proper specular maps to correctly reflect the environments.

[**The Halls of the Greybeards - A High Hrothgar Retexuring v1.01**](https://www.nexusmods.com/skyrimspecialedition/mods/22672?tab=files): A retexturing of High Hrothgar. There are 4 versions. A standard version with 4k diffuse and 2k normals, 4k diffuse and 4k normals and a dark version with 4k diffuse and 2k normals, 4k diffuse and 4k normals. This mod fixes a ton of texture layout issues within the meshes too.
- If using "Skyrim Textures Redone - High Hrothgar", remove "hhintbaycol01.dds" and "hhintbaycol01_n.dds" from the following path:  \The Halls of the Greybeards - a High Hrothgar Retexuring\textures\architecture\highhrothgar.  This will allow the STR mod's superior texture to take precedence.  

[**Skyland Imperial and Nordic Tents v1.6**](https://www.nexusmods.com/skyrimspecialedition/mods/57002?tab=files): Skyland Imperial and Nordic Tents introduces 4k tent textures for Nordic and imperial tents. Skyland tents offers a brand new mesh for the large Nordic fur tent for better visuals.

[**Water in Wells - Mesh-only Animated Wells v0.7**](https://www.nexusmods.com/skyrimspecialedition/mods/57268?tab=files): A mesh-only solution for animated water in wells and sewers. No ESP. 

[**Clothing Iron - 4K v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/53247?tab=files): Remesh and 4K retexture of the clothing iron.

[**TB's Silver Ingot 4K v8.0**](https://www.nexusmods.com/skyrimspecialedition/mods/60841?tab=files): Adds a new cube map, diffuse and normal to the Silver Ingot - Available in 4K and 2K resolutions.

[**TB's Wine 4K Version v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/61131?tab=files): This is a retexture containing no ESPs which comes in 3 Variants - 2K, 4K and 8K and aims to improve upon the default Skyrim textures, thank you very much for considering my mod (Also introduces some transparency into the glass).

[**Cork Retexture v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/41903?tab=files): Cork retexture. 4x the size of vanilla's.

[**Dibella Statue v1.04**](https://www.nexusmods.com/skyrimspecialedition/mods/61553?tab=files): Dibella statue replacer.
- Delete ESP file.

[**High Quality Food and Ingredients SE v1.9**](https://www.nexusmods.com/skyrimspecialedition/mods/10897): HQ textures of the food and ingredients for Skyrim Special Edition.

[**Business Ledger HD Retexture v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/67319): This is an HD retexture of the Business Ledger by LamboMan ported with permission ("Please go ahead, you can do whatever you need with it"). 

[**Handcarts SE - Everything changes v0.3**](https://www.nexusmods.com/skyrimspecialedition/mods/76672): It's been a long time, a lot has changed in Skyrim, but finally completely new handcarts started appearing on the streets.

[**burlap01.dds by Xtudo v0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/76672): This archive contains a wonderful and very atmospheric canopy texture burlap01.dds provided by Xtudo.

[**Rudy HQ - Miscellaneous SE v1.02**](https://www.nexusmods.com/skyrimspecialedition/mods/19867): HQ meshes for a glazed pottery with a new 4K/2K textures. HQ meshes for in-game silverware with a new HQ candles. Realistic apples, tomatoes, potatoes, and a common bed pillows, plus HQ meshes for a common plates.

[**No More Hanging Moss v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/16426): Effectively removes hanging moss from the game world with a mesh edit and optional esp. 

[**CC's UHD Coal Piles v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/44851): A simple mod that remakes the coal piles next to the smelters in 8K. Also available in 4K, 2K and 1K.

[**Kanjs - Bird Nests and Eggs - up to 4k v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/64905?tab=files): Kanjs - Nests and Eggs is a mod that retexture all bird nests, eggs and remeshes all nests!

[**Kanjs Nests Egg Harvesting Fix v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/79026?tab=files): This is a mesh replacer for the eggs in Kanjs nests mod. When you harvest this mesh, one egg is removed in keeping with the amount of eggs you receive.

[**Dwarven Arrows and Bolts Revamped Texture 4k - 2k v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/2927?tab=files): A finely etched, richly detailed re-imagined texturing work of the Dwarven arrows and quiver. I put many hours of care and work to create something aesthetically beautiful so I can be enthralled by firing a reign of arrows upon my foes in glorious 4k :) Enjoy!

[**Terrain LOD for Septentrional Landscapes v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/39563): New overhaul for Terrain LOD landscape textures that corresponds with the texture mods you have installed..
- Only used for terrain noise texture.  Remove ALL files except for the \textures\ folder.

[**CC's HQ Mines Redone - AiO v1.5**](https://www.nexusmods.com/skyrimspecialedition/mods/18044): This is a retexture of the Mines in skyrim. All textures handmade by me using Substance Designer 2018.

[**CC's HQ Mines Redone Parallax Textures v2.6**](https://www.nexusmods.com/skyrimspecialedition/mods/51261): Parallax Textures for CC's HQ Mines Redone.
- Remove \textures\smim\ folder to prevent conflicts with other mods.

[**Skyrim Remastered - Caves 4K Parallax v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/38220/?tab=files): A retexture of Skyrim's caves, with a complete overhaul for the ice caves to make them look like actual ice. Offered in 4k, 2k, and 1k texture quality with parallax options.

[**CC's HQ Caves - 2K v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/8448?tab=files): This is a retexture of the Cavewalls and the Cavefloor. All textures handmade using Substance Designer 6.

[**CC's HQ Caves Parallax Textures for Skyrim Remastered - Caves v2.2**](https://www.nexusmods.com/skyrimspecialedition/mods/44877?tab=files): Parallax textures for CC's HQ Caves; requires Skyrim Remastered - Caves and SSE Parallax Shader Fix.

[**Skyrim Textures Redone - High Hrothgar Parallax v2.5**](https://www.nexusmods.com/skyrimspecialedition/mods/51403?tab=files): Parallax Meshes and Textures for Skyrim Textures Redone - High Hrothgar and SkyHaven. 

[**Skyrim Textures Redone - SkyHaven Parallax v2.5**](https://www.nexusmods.com/skyrimspecialedition/mods/51403?tab=files): Parallax Meshes and Textures for Skyrim Textures Redone - High Hrothgar and SkyHaven. 

[**4K Parallax High Hrothgar by Pfuscher - Update1 v1.0**](https://www.nexusmods.com/skyrim/mods/58938?tab=files): Thanks and props to VoltarDaedra.

[**Boreal Boats Parallax Meshes SE v1.3**](https://www.nexusmods.com/skyrimspecialedition/mods/47608?tab=files): Required for Parallax Effect.

[**Pelt by Pfuscher v1.0**](https://www.nexusmods.com/skyrim/mods/65981?tab=files): High Res Pelt with Parallax.

[**Skyrim 2020 Parallax by Pfuscher - 2K v8.4.2**](https://www.nexusmods.com/skyrimspecialedition/mods/2347?tab=files): High Res Textures for cities, dungeons, clutter, armors, landscapes and much more. Going towards 2000 files, way more to come!  This mod has over a thousand hours of work put into it. If you enjoy my work please consider supporting me at Patreon and / or Kofi.
- Not safe to use complete texture pack with Enderal VR.
- Do not update as the newest pack seems to break parallax effects.
- Currently using ONLY \textures\architecture\farmhouse, \textures\landscape\roads, and \textures\landscape\trees which have been fully tested.

[**Parallax Mesh Collection v2.02**](https://www.nexusmods.com/skyrimspecialedition/mods/2347?tab=files): Patches to add parallax to meshes.
- Not safe to use complete mesh pack with Enderal VR.
- Currently using ONLY \meshes\architecture\farmhouse, \meshes\clutter\ruins\ruinspuzzlepillar*.nif, and \meshes\landscape\trees which have been fully tested.
- Remove \meshes\architecture\farmhouse\fencewoven*.nif to prevent 'SD's Farmhouse Fences SE' from being overrided.
- Remove \meshes\architecture\farmhouse\farmwell01.nif to prevent 'Water in Wells' from being overrided.

[**Chicken Replacer - Mihail Monsters and Animals (SE-AE version) (''bird'') v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/76452): High quality vanilla Chicken replacer: make these birds finally worthy of having the entire population of Skyrim committed to their protection.

[**High Poly Mudcrab N Retexture v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/62967?tab=files): Pfuscher's High Poly Mudcrabs N Retexture.

[**FusaFusa Project - Fluffy Animals SE v14.2**](https://www.nexusmods.com/skyrimspecialedition/mods/5514?tab=files): Increase Fur Volume of Animals. They become more fluffy.

[**Fluffworks Medium v1.1f**](https://www.nexusmods.com/skyrimspecialedition/mods/56361?tab=files): Enhanced fur on animals using shell texturing.
- Recommend deleting the optional ESP file.
- Remove "Horse.nif" as this causes texture problems with select horses.

[**Fluffworks - Better Photoreal Foxes v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/65974?tab=files): A makeover for Skyrim's Foxes, Combining Better Foxes & Photoreal Foxes with Fluffworks Shell Texturing on top!

[**Smaller Insects v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/51551?tab=files): This mod aims to resize the scale of animals in Skyrim to give a better immersive feelig in VR / First person.

[**Better Dwemer Spider Textures 4096 Pixel Standard v1.1**](https://www.nexusmods.com/skyrim/mods/51270?tab=files): Get your Dwemer Spiders ready for their closeups with these brilliant and astounding new textures, built from the ground up with top-quality Dwarven Ingots and entirely too many Photoshop layers. Guaranteed to improve spider productivity by up to 42 percent.
- Needs processed by Cathedral Assets Optimizer with the following settings enabled: Process meshes, Full optimization, Always process headparts, Resave meshes. Process textures, necessary optimization, Compress textures, Generate mipmaps.  

[**KS Hairdos SSE v1.9**](https://www.nexusmods.com/skyrimspecialedition/mods/6817?tab=files): KS Hairdos is a hair pack that contains 922 hairstyles. 830 hairstyles are for females, 92 are for males.

[**Caliente's Beautiful Bodies Enhancer - CBBE v1.7.1**](https://www.nexusmods.com/skyrimspecialedition/mods/198?tab=files): A completely customisable female body replacer for TESV: Skyrim.

[**Bijin Skin - CBBE v1.4**](https://www.nexusmods.com/skyrimspecialedition/mods/20078?tab=files): Skin textures for CBBE and UNP made by rxkx22.
- Installed with default settings with "4K - Wet" specular maps.

[**Deadly Spell Impacts v1.7**](https://www.nexusmods.com/skyrimspecialedition/mods/12939?tab=files): Fire, lightning, frost, and spit (Spider/Chaurus) spell impacts now have their own unique textures. This mod also increases the variation in impact size, increases the size of dragon breath impacts, and adds melted snow impacts for fire and lightning spells.

[**Visual Animated Enchants v0.2**](https://www.nexusmods.com/skyrimspecialedition/mods/7037?tab=files): A replacer for the visual and animation of the enchantments on weapons to make them more magical and immersive.  
- Remove "Cell" data in xEdit.

[**Qwinn's Refined Visual Animated Enchants v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/24665?tab=files): With L3stat's kind permission, a refinement and fix for various issues with Visual Animated Enchants.

[**Adjusted Visual Animated Enchants (No ENB Complex Particle Lights) v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/50382?tab=files): Tweaks the appearance of enchantments from Visual Animated Enchants. Reduces size and brightness to work better when using ENB, alters flame mesh shapes on unique weapons to fit more closely, and adjusts some colours.

[**Dynamically Disable Eye Adaptation and Bloom v1.2.0**](https://www.nexusmods.com/skyrimspecialedition/mods/2135?tab=files): Disables the irritating eye adaptation and object blooming through scripting. Compatible with all image space lighting mods!

[**Smoking Torches and Candles SSE v1.76**](https://www.nexusmods.com/skyrimspecialedition/mods/8607): A modification that adds a smoke particle effect to torches used by the player and the NPCs as well as those mounted to the wall. Optional component will add a smoke particle effect to most candles in the game world.
- Added for smoking candles.  Smoking torches appears to not always function.

[**Storm Lightning for SSE and VR v1.4.17**](https://www.nexusmods.com/skyrimspecialedition/mods/29243?tab=files): A remake of Minty's Lightning mod as an SKSE plugin. The purpose of this mod is stability and scalability. It can summon up to 50 sheet lightnings and 50 fork lightnings per second and up to 31 cells distance. This results in a more natural and enjoyable storm experience.

[**Pouring Rain v2.0**](https://www.nexusmods.com/skyrimspecialedition/mods/6077?tab=files): Increases rain particles density during raining weathers.

[**R.A.S.S - Rain Ash And Snow Shaders v3.2.2**](https://www.nexusmods.com/skyrimspecialedition/mods/22780?tab=files): "R.A.S.S." adds visual effects to the Player and NPCs during certain conditions.

[**R.A.S.S Cold Breath for Enderal v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/271?tab=files): Modified the R.A.S.S plugin so the cold breath effect works in Enderal's colder regions.
- This plugin appears to have a bug where the Ash FX are constantly active.  To fix this, remove "Visual Effect.RASS_CameraFX_Ash_Visual" and "Effect Shader.RASS_FX_Ash" from the plugin with xEdit.

[**Simplicity of Snow v0.10**](https://www.nexusmods.com/skyrimspecialedition/mods/56235?tab=files): A light-weight snow mod designed to minimize conflicts. Uses your own snow texture and removes snow from under roofs.
- Remove the plugin's "Static.DirtCliffs03Snow01Snow" data in xEdit.

[**SkyVRaan - Shimmering VR Waters v1.0.1**](https://www.nexusmods.com/skyrimspecialedition/mods/30571?tab=files): Adds a fake reflection effect to Skyrim VR's outdoor water. It breaks up the distant LOD, shows wave movement on the distant water, and gives an illusion of water depth in the distance. Also has improved realism and clarity of near water.
- During the installation, tick "Rally's Water Foam (4K)" and "Improved Water Normals for Vanilla" and leave all other settings at default.  Do NOT install Rocky Riverbeds due to high performance drop.
- Recommend replacing 'OutputCube.dds' with 'ewpdefault.dds' from the [Enhanced Wetness and Puddles](https://www.nexusmods.com/skyrimspecialedition/mods/58155?tab=description) mod for improved water reflections.
- Do not update to the new DLL version of the mod. Enderal VR requires Synthesis patching.

[**3D World Fog Map v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/340?tab=files): Add fog back to the 3D world map!

[**Nyghtfall - Dark Fantasy Music for Enderal v1.0.0**](https://www.nexusmods.com/enderalspecialedition/mods/425): Adds new exploration and combat music tracks from Nyghtfall - Dark Fantasy Music to Enderal.

[**Nyghtfall - Combat Music Fix v1.0.1**](https://www.nexusmods.com/enderalspecialedition/mods/425): Fixes missing combat music conditions.

[**Myths and Legends VI - The Forgotten One v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/25?tab=files): Adds a new Myths and Legends book, a new dungeon, and a completely new creature with unique mechanics.

[**Yero's Cave Full v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/376?tab=files): Enhances Yero's cave by adding an unique boss and exchanges the way of how soul gems are filled.

[**Fire of the Mountain SE v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/377?tab=files): This is the translation of a very nice quest mod. I've either enhanced it a bit as there were some slight issues.

[**Playable Half Starling Race v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/100?tab=files): Adds Half Starlings as a playable race.

[**Starlings Leveled v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/132?tab=files): Adjusts the Starlings to level with the player.

[**Old Tunnel Pathing Fix v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/143?tab=files): Fixes pathing issues in the Suncoast dungeon "Old Tunnel". (Trolls no longer flee from the player)

[**NPC Pathing Fixes (Suncoast) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/303?tab=files): Improved the NPC pathing and added new areas that are now path-able in the Sun Coast.

[**NPC Pathing Fixes (Heartland) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/379?tab=files): Improved the NPC pathing in the Heartland.

[**NPC Pathing Fixes (Whisperwood) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/380?tab=files): Improved the NPC pathing in the Whisperwood.

[**Suncoast Enemy Placement Redone v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/387?tab=files): Removes encounters, removes enemies from encounters, and moves enemies around.

[**Delectable Docks SE v1.2**](https://www.nexusmods.com/enderalspecialedition/mods/77?tab=files): Adds many details to the docks and harbors of Enderal focused on improving immersion.

[**Delectable Docks SE - ESP Fix v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/77): SE port of my delectable docks mod.

[**Dust Pit Revised v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/307?tab=files): Immersive rework of Dust Pit Arena.

[**Center of the Earth v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/196?tab=files): Follow Yaronth of Aran's ill-fated expedition to the center of the earth.

[**Undercity Home v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/146?tab=files): A simple place for you to sleep in the Undercity - ported to SE.

[**Beach House v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/145?tab=files): There is an abondoned house at the Sun Coast beach for you to explore and occupy as a player home.

[**White Hearth - Enderal SE v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/137?tab=files): A new player home near Ark (port to SE).

[**Tamira's Enderal Log Cabin SE - Player Home v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/114?tab=files): A small player home near Riverville.

[**Noble Quarter Player Home Redone v1.03**](https://www.nexusmods.com/enderalspecialedition/mods/66?tab=files): Overhauls player home in Nobles Quarter.

[**Patch for Mandragorasprouts' Noble Quarter Player House Redone mod v0.1**](https://www.nexusmods.com/enderalspecialedition/mods/117?tab=files): This mod will fix Display Cases in both Player Homes (Ark Marketplace & Noble Quarter) so they actually work.

[**Meditation Area Fixes v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/265?tab=files): Fixes some issues in the meditation area.

[**EOP SE - Enderal SE Outposts v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/18?tab=files): Adds order outposts, fortifies some camps with additional protection. 

[**Riverville Catacombs SE v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/80?tab=files): Forgotten Dungeons implements cut content, originally made by SureAI, with updates and fixes to fit seamlessly into the game.

[**Enderal SE - Undercity Arena Fix v.1.02**](https://www.nexusmods.com/enderalspecialedition/mods/9?tab=files): Reworks the undercity arena to be less cheeseable, bigger and fixes an issue with shadows.

[**Forgotten Dungeons - Abandoned Excavation Site v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/110): Forgotten Dungeons implements cut content, originally made by SureAI, with updates and fixes to fit seamlessly into the game.

[**Frostville SE v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/127?tab=files): A small but functional settlement overhaul for the Frostcliff Tavern.
- Do not update to v1.03.  Incompatible with Enderal VR.

[**Thalgard Monastery v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/133?tab=files): Forgotten Dungeons implements cut content, originally made by SureAI, with updates and fixes to fit seamlessly into the game.

[**EAM SE - Enderal Apothecarii Monastery v1.05**](https://www.nexusmods.com/enderalspecialedition/mods/34?tab=files): Adds the Apothecarii Monastery including: Huge monastery area, over 10 interiors, 2 dungeons and much more.

[**Golden Mare Mill SE v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/142?tab=files): Golden Mare Mill provides a quaint player home in the scenic area of Riverville which is rewarded for the completion of the quest "Secrets from the Can".

[**Wellwatch Manor SE v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/151?tab=files): Adds a proper outpost to the Wellwatch myrad tower and a purchasable player home.

[**Riverville Jail SE v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/157?tab=files): Expands upon the Riverville Jail by adding a watchtower, a secret exit and more.

[**Bank of Ark SE v1.04**](https://www.nexusmods.com/enderalspecialedition/mods/158?tab=files): Adds new models for corridors, vault doors/vault door numbers and makes some changes to the interior of the Ark Bank.  

[**Seaview Lodge SE v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/188?tab=files): Seaview Lodge adds a player home in the scenic area of the sea near Ark.

[**Forgotten Dungeons - Palm Cove v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/272?tab=files): Forgotten Dungeons implements cut content, originally made by SureAI, with updates and fixes to fit seamlessly into the game.

[**Storeable Phasmalist Talismans v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/68?tab=files): Allows you to store away Phasmalist Talismans.
- Do not install 2.0.12 update.

[**Unique Armor Sets Replacer Enderal SE v2.3**](https://www.nexusmods.com/enderalspecialedition/mods/27?tab=files): High-quality and lore friendly replacers for many of Enderal's unique armor sets! Converted with SSE nif optimizer.

[**Dawnguard Heavy Armor (Shadowsteel Brigandine) - SE v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/33?tab=files): A port of Dawnguard heavy armor set from Skyrim SE to Enderal SE.

[**Practical Armor Replacers v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/23?tab=files): Armor and weapons more fitting to the setting of Enderal. Converted to SE!

[**Kolapon's Brand New Armor Sets and Weapons SE v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/364?tab=files): Adds brand new sets of armor and weapons to different locations in Enderal.

[**Unique Amulets and Masks (Ancient and Qalians Last Smile) SE v1.2**](https://www.nexusmods.com/enderalspecialedition/mods/363?tab=files): Gives unique models to some of the rare amulets, the Ancient mask and Qalian's Last Smile.

[**Unique Amulets and Masks SE Fixes v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/365?tab=files): Fixes some things related to SE updates.

[**Pumpkin Fixes v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/399): Fixes some issues related to Pumpkins and related plants. 

[**Moddable Iron-Steel Weapons v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/341): This fixes issues with weapon replacer mods that replace iron and steel weapons.

[**Moddable Iron Armor v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/392?tab=files): This fixes issues with armor replacer mods not replacing iron armor.

[**Enderal SE - Crossbows v1.07**](https://www.nexusmods.com/enderalspecialedition/mods/4?tab=files): Adds Crossbows to Enderal SE.

[**Unique Enderal Uniques SE v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/38?tab=files): Enderal SE conversion of Unique Enderal Uniques using SSE nif optimizer.

[**Kolapon's Unique Weapons v1.5**](https://www.nexusmods.com/enderalspecialedition/mods/95?tab=files): Gives unique appearance to several of the unique weapons in Enderal and adds a brand new staff to one of the bosses.

[**Sting of the Blue Islands Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/86?tab=files): Replaces that Ugly Scimitar with something worthy of betraying the Golden Sickle for.

[**Bowgasm SE - Nicos AIO Vanilla Bow Replacer SE v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/42929?tab=files): Optional file is a non-plug in replacer for nearly all Vanilla bows in game with higher poly models, more realistic shapes, and higher resolution textures.

[**Steel Swords Redone v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/18670/?tab=files): This mod adds new models and textures for the steel sword and steel greatsword.

[**Iron Things v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/26947?tab=files): Replacer meshes and textures for IRON THINGS: iron sword, greatsword, dagger, battleaxe, bow, and shield. Stand-alone is also available for download. Made in 2016 by ClipsyMoon, now on SE for all to enjoy. ;)

[**Maps - SE v1.2**](https://www.nexusmods.com/enderal/mods/49?tab=files): You can now buy maps that will show you the landmarks of the region.

[**Ark Wasserspeier - Ark Watersprouts (SE) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/62?tab=files): Changes the waterspouts in the Foreign Quarter in Ark.

[**Waterspout Fixes v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/374?tab=files): Fixes some things from the Waterspouts mod.

[**Drunken Bee Sign v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/118): Adds a sign to the blank wall on the exterior of the Drunken Bee in Riverville.  

[**Enderal VR Main Menu Logo v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/397?tab=files): Enderal logo for the Enderal VR Main Menu.

[**Static Mushrooms  - High Poly SE v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/129?tab=files): Many animated/interactive/static mushrooms across Enderal are high poly now.
 
[**Craftsman Tools Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/28?tab=files): Replaces meshes and textures of the crafting tools seen throughout Enderal.

[**Cannons 2K v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/63?tab=files): Replaces the cannons and cannonballs with new 2K textures.

[**The Notice Board Redefined for Enderal v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/153?tab=files): Replaces low quality notes on bounty boards with notes from The Notice Board Redefined.

[**Enderal Distinctive Clothing v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/348?tab=files): Distinctive retextures for clothing.

[**Enderal Distinctive Jewelry v1.5**](https://www.nexusmods.com/enderalspecialedition/mods/370?tab=files): Distinctive models and textures for jewelry.

[**Akropolis Stones Remastered v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/488): Fully retextured stone and pillar textures in Akropolis, with HD and realistic material properties, in order to be as detailed and interesting to look at as possible.

[**Conduit - Short-term Weapon Infusions v2.7**](https://www.nexusmods.com/skyrimspecialedition/mods/58023?tab=files): When holding a weapon in one hand and a spell in the other, you are able to temporarily "conduct" the spell through that weapon. Different categories of spells make the weapon do different things. This effect will overlay on top of normal enchants and does include additional weapon FX that will overlay too. It even works on Bound weapons.

[**Conduit - Enderal Adaption Patch v2.5-EA1**](https://www.nexusmods.com/skyrimspecialedition/mods/58023?tab=files): This is an experimental rebalance (read: heavy nerf) of the mod for Enderal. If you feel Conduit is overtuned for normal Skyrim, you can use this patch there as well, it doesnt require Enderal. ESL-flagged.

[**Enhanced Blood Textures Enderal SE v4.0**](https://www.nexusmods.com/enderalspecialedition/mods/360?tab=files): A blood overhaul mod.

[**Less Grass 1 - 50% Less v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/69?tab=files): Reduces the density of grass for better visibility.

[**Weather Fixes v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/278?tab=files): Fixes some issues with Enderal weathers which increases compatibility with some weather-related mods. (e.g. R.A.S.S., Storm Lightning)
- Load Order Recommendation: Weather Fixes, Diverse Weather, True Storms, Diverse Weather SE - True Storms, Intense Sandstorms.

[**Diverse Weather v1.12**](https://www.nexusmods.com/enderalspecialedition/mods/70?tab=files): Diversifies the weather in Enderal and adds a few new ones.

[**True Storms Special Edition - Thunder Rain and Weather Redone v1.0.2**](https://www.nexusmods.com/skyrimspecialedition/mods/2472?tab=files): True Storms Special Edition is a complete overhaul of the storm systems in Skyrim SE, including new heavy and unique weathers, loads of new intense sound effects, interior sounds, particle effects, new rain, snow, and dust textures, heavy fogs, new weathers for Solstheim including dust storms, and much more!

[**Enderal SE - True Storms v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/203?tab=files): Compatibility patch for True Storms.

[**Intense Sandstorms v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/279?tab=files): Increases the intensity of sandstorms in the Desert.

[**Dirt and Blood - Dynamic Visual Effects v2.24**](https://www.nexusmods.com/skyrimspecialedition/mods/38886?tab=files): Your character will accumulate dirt and blood dynamically, which you can clean by swimming or standing in the rain. The effects are mostly visual only and do not affect gameplay. NPCs will also get bloody as a result of battles. Mod is designed to be simple and lightweight.
- Remove "Wash and Rinse" from the plugin's Spell data and set 6E00082F records to 0 from Quest.Dirty_Quest and Quest.DirtyQuesMCM using xEdit to completely remove the broken "Wash and Rinse" spell from the mod.

[**Enderal SE - Dirt and Blood v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/201?tab=files): Compatibility patch for Dirt and Blood.

[**Frozen Electrocuted Combustion - v5.1**](https://www.nexusmods.com/skyrimspecialedition/mods/3532?tab=files): Applies visual effects to NPCs and the player, when killed by magic status effects.
- Remove optional DLL.

[**Frozen Electrocuted Combustion VR v5.1**](https://www.nexusmods.com/skyrimspecialedition/mods/59118?tab=files): Applies visual effects to NPCs and the player, when killed by air, ash, dragons, drain, fire, frost, fear, lightning, poison, soultrap, steam and sun damage status effects. VR version that requires original FEC to run

[**Enderal SE - Frozen Electrocuted Combustion v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/505?tab=files): Compatibility patch for Frozen Electrocuted Combustion.

Required load order:
* VR Address Library for SKSEVR
* powerofthree's Papyrus Extender 
* Papyrus Extender VR
* Frozen Electrocuted Combustion 
* Frozen Electrocuted Combustion VR
* Enderal SE - Frozen Electrocuted Combustion

[**Enderal NPC Overhaul - SE version v2.3.1**](https://www.nexusmods.com/enderalspecialedition/mods/150?tab=description): Overhaul of all NPCs in Enderal. Most important NPCs are given unique look (100+), others - KS Hairdos Hair. NO ESP. No requirements.

[**Kids of Enderal - SE v1.7**](https://www.nexusmods.com/skyrim/mods/93432?tab=files): Remakes kids in Enderal to look like Skyrim's "The Kids are Alright".

[**Stronger Souls v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/113?tab=files): Makes the conjured Souls stronger. 

[**Stronger Summons v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/202?tab=files): Makes your summoned creatures stronger.

[**Tharael's Afterlife v2.0**](https://www.nexusmods.com/enderalspecialedition/mods/45?tab=files):  The mod adds an option to make Tharaêl your companion after completing Dark Chambers of Our Mind (providing that you sided with him). It also changes the side room in the house in the Nobles Quarter.

[**Amanda v1.4.2**](https://www.nexusmods.com/enderalspecialedition/mods/15?tab=files): Adds female follower to The Drunken Bee tavern in Riverville.

[**A Follower Named Ishan v1.2**](https://www.nexusmods.com/enderalspecialedition/mods/327?tab=files): Adds a custom voiced Qyranian follower at the Drunken Bee in Riverville.

[**Jespar Has Steel SE v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/239?tab=files): Jespar no longer uses toothpicks in battles of life and death.

[**Calia and Jespar Visual Overhaul v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/472?tab=files): High poly heads for our beloved followers and love interests. Heavily based on their original looks.

[**Face Discoloration Fix VR v1.0.3**](https://www.nexusmods.com/skyrimspecialedition/mods/42441?tab=files): Eliminates the dreaded "dark face" issue that occurs when the game encounters FaceGen errors.

[**Seagulls of Skyrim v1.4**](https://www.nexusmods.com/skyrimspecialedition/mods/52153?tab=files): This mod adds seagulls along the coasts of Skyrim and Solstheim, with animated models and sounds from Mr. Siika Seagulls for Skyrim SE!

[**Enderal SE - Seagulls of Skyrim v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/204?tab=files): Compatibility patch for Seagulls of Skyrim which adds them to the world of Vyn.

[**Flying Crows SSE v1.2**](https://www.nexusmods.com/skyrimspecialedition/mods/49270?tab=files): Adds flying crows to various locations around Tamriel to create a more nordic atmosphere in your Skyrim.

[**Enderal SE - Flying Crows v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/205?tab=files): Compatibility patch for Flying Crows which adds them to the world of Vyn.

[**Bears of the North v1.1**](https://www.nexusmods.com/skyrimspecialedition/mods/47541?tab=files): Visual overhaul of the bears of Skyrim. Bigger, badder bears fit for the harsh northern lands they roam.

[**Enderal SE - Bears of the North v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/30?tab=files): Enderal SE compatibility patch for Bears of the North.

[**Creature Replacer Pack v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/74?tab=files): A collection of creature replacers for Enderal converted to SE.

[**Enderal - Arp v2.12**](https://www.nexusmods.com/enderalspecialedition/mods/36?tab=files): Completely redesigned 4K Arps for Enderal SE and VR.

[**Enderal - Vatyr v5.0**](https://www.nexusmods.com/enderalspecialedition/mods/41?tab=files): Completely redesigned Vatyr in 4K for Enderal SE and VR.

[**Enderal - Donkey v2.61**](https://www.nexusmods.com/enderalspecialedition/mods/107?tab=files): Enderal replacer. This changes the textures of donkey.nif & donkey_barrel.nif, custom variations on every donk.

[**Boneripper Replacer (Clannfear) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/59?tab=files): Replaces the models Bonerippers with high quality alternatives.

[**Pus Beetle Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/48?tab=files): Replaces the models Pus Beetles with high quality alternatives.

[**Kolapon's Various Creatures Replacers v1.5v**](https://www.nexusmods.com/enderalspecialedition/mods/64?tab=files): Changes the appearance of some of the creatures so they are unique to Enderal.

[**Enderal SE - Predators v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/115?tab=files): Replaces the models of Panthers, Leopards and Shadow/Mountain Deerstalker with alternatives.

[**Deerstalker (Sabrecat) Replacer v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/122?tab=files): Replaces the Deerstalker (Sabrecat) models with high quality alternatives.

[**Deerstalker Redone v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/122?tab=files): Renames Mountain Deerstalker and Shadow Deerstalker to Shadow Stalker and adds appropriate loot.

[**Frost Troll Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/121?tab=files): Replaces the model of Frost Trolls with high-quality alternatives.

[**Oorbaya Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/296?tab=files): Replaces the models Oorbayas with high quality alternatives.

[**Arvak Replace SE v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/24929?tab=files): Arvak Replace.
- Delete ESP file.

[**Shadow of Transcience Mount Fix v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/381?tab=files): Replaces the original model with a new one which fixes a lot of issues.
- Do not install 2.0.12 update.

[**Shadow of Transcience Mount Fix Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/382?tab=files): Replaces the model of Shadow of Transciense if the Mount Fix is used.

[**Kolapon's Undead Creatures Replacers v1.2u**](https://www.nexusmods.com/enderalspecialedition/mods/64?tab=files): Changes the appearance of some of the creatures so they are unique to Enderal.

[**Ancestral Spirit Replacer (Variant 2) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/60?tab=files): Replaces the models Ancestral Spirits with high quality alternatives.

[**GoT Dragon in Enderal - Drogon v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/497?tab=files): Replace that Enderal dragon with Drogon, Rhaegal or Viserion.

[**XP32 Maximum Skeleton Special Extended - XPMSSE v4.81**](https://www.nexusmods.com/skyrimspecialedition/mods/1988?tab=files): XP32 Maximum Skeleton Special Extended is the update of XP32 Maximum Skeleton Extended for Skyrim Special Edition.

[**Enderal Armor and Weapon Overhaul v2.0**](https://www.scenicroute.games/projects/somnium): This mod changes almost every piece of armor and weapon in the game. And some clothes. No more Skyrim flashbacks in Enderal.

[**Enderal Armor and Weapon Overhaul - Replacer v1.14**](https://www.scenicroute.games/projects/somnium): Apoapse's Accoutrement patch for EAWO.

[**EGO SE - Enderal Gameplay Overhaul v1.89**](https://www.nexusmods.com/enderalspecialedition/mods/3?tab=files): This is a complete overhaul of the gameplay mechanics of Enderal. This includes a ton of balance changes, improvements to the ai, new gameplay mechanics, new weapons/spells/potions and much more. (ENG/GER/RUS)
- Do not install 2.0.12 update.
- Remove "Game Setting".fAutoAimMaxDegrees, "Game Setting".fAutoAimMaxDistance, and "Game Setting".fAutoAimScreenPercentage in xEdit to fix targeting reticules for VR.
- Delete \EGO SE - Enderal Gameplay Overhaul\scripts\ _00e_a0_banksystemquest.pex to fix problems with banking system in VR.

[**EGO SE - Myths and Legends VI - The Forgotten One v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/25?tab=files): A balance patch for Enderal SE Gameplay Overhaul. Compatible with all languages.

[**EGO - Fire of the Mountain v1.0**](https://www.nexusmods.com/enderal/mods/186?tab=files): Balanced for EGO, some small translation fixes, added EGO enemy perks/abilities to enemies.

[**EGO SE - Playable Half Starling Race v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/100?tab=files): Adds Half Starlings as a playable race. (ENDERAL GAMEPLAY OVERHAUL VERSION) Only download one of the files.

[**EGO SE - Thalgard Monastery v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/133?tab=files): Compatibility patch for Enderal Gameplay Overhaul. (ENG/GER/RUS)

[**EGO SE - EAM SE - Enderal Apothecarii Monastery v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/34?tab=files): Compatibility patch for Enderal Gameplay Overhaul.

[**EGO SE - Wellwatch Manor SE v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/151?tab=files): Replaces the Secure Chest with an EGO Secure Chest. (not needed if you use the secure chest optional patch) Load EGO patch after the main file and before the translation file!

[**EGO SE - Riverville Jail SE v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/157?tab=files): Compatibility patch for Enderal Gameplay Overhaul.

[**EGO SE - Bank of Ark SE v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/158?tab=files): Compatibility patch for Enderal Gameplay Overhaul.

[**EGO SE - Meditation Area Fixes v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/265?tab=files): Enderal Gameplay Overhaul Version. Only download one of the files.

[**EGO SE - Unique Amulets and Masks v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/366?tab=files): Compatibility patch for Enderal Gameplay Overhaul and Unique Amulets and Masks.

[**EGO SE - Moddable Iron Armor v1.00**](https://www.nexusmods.com/enderalspecialedition/mods/392?tab=files): Enderal Gameplay Overhaul Version. Only download one of the files.

[**EGO SE - Moddable Iron-Steel Weapons v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/341?tab=files): Enderal Gameplay Overhaul Version. Only download one of the files.

[**EGO SE - Even More Unique Weapons v1.02**](https://www.nexusmods.com/enderalspecialedition/mods/124?tab=files): Compatibility patch for Enderal Gameplay Overhaul and Even More Unique Weapons. (ENG/GER/RUS)

[**EGO SE - Bears of the North v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/30?tab=files): Enderal Gameplay Overhaul version. (Only download this or the other)

[**EGO SE - Deerstalker Redone v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/122?tab=files): Renames Mountain Deerstalker and Shadow Deerstalker to Shadow Stalker and adds appropriate loot.

[**EGO SE - Donkey v1.1.1**](https://www.nexusmods.com/enderalspecialedition/mods/125?tab=files): Compatibility patch for Enderal Gameplay Overhaul and Enderal - Donkey. (ENG/GER/RUS)

[**EGO SE - Kolapon's Undead Creatures Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/342?tab=files): Compatibility patch for Enderal Gameplay Overhaul and Kolapon's Undead Creatures Replacer.
- Do not install 2.0.12 update.

[**EGO SE - Kolapon's Various Creatures Replacer v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/351?tab=files): Compatibility patch for Enderal Gameplay Overhaul and Kolapon's Various Creatures Replacer.

[**EGO SE - No more Skyrim-looking Creatures EGO Patch v1.1**](https://www.nexusmods.com/enderalspecialedition/mods/181/?tab=files): Patch between for No More Skyrim-looking Creatures and EGO.

[**Enderal - Gameplay Overhaul - EAO Patch v1.0**](https://www.scenicroute.games/projects/somnium): This is a patch for Enderal Gameplay Overhaul and Enderal Armor and Weapons Overhaul.

[**Enderal - Gameplay Overhaul - EWO Patch v1.0**](https://www.scenicroute.games/projects/somnium): This is a patch for Enderal Gameplay Overhaul and Enderal Armor and Weapons Overhaul.

[**Apoapse's Accoutrement v1.1.1**](https://www.scenicroute.games/projects/somnium): Weapons and armor have been totally remodeled, with assets pulled from dozens of excellent Skyrim mods, to match our “Age of Sail” theme. Most outfits have been hand-selected for different NPCs, both generic and unique, to fit the setting.
- Removed ComelyCoiffures_EN.esp, Engarde.esp, TERAArmorsSSE.esp as Masters in xEdit. (Replace with blank ESP, remove errors in plugins, then Clean Masters.)

[**Prime Fixes Collection v1.1.1**](https://www.scenicroute.games/projects/somnium): Fixes pauldrons in Apoapse's Accoutrement. 
- Remove all "Primes_Fixes_v2.esp" entries in xEdit with the exception of Armor Addon, Armor, and Outfit entries which override Apoapse's Accoutrement.

[**Screw the Black Guardian V2 v1.0**](https://www.scenicroute.games/projects/somnium): Replaces the Black Guardian fight with a more morally grey decision you have to make, and the whole scene is streamlined without cutting out the quality of the dialogue and exposition.
- Removed Apoapse's Arsenal.esp as Master in xEdit. (Replace with blank ESP, remove errors in plugins, then Clean Masters.)

[**Somnium Music Edits v1.0**](https://www.scenicroute.games/projects/somnium): New music for main menu.

[**Somnium Retextures v1.1.1**](https://www.scenicroute.games/projects/somnium): Textures/meshes for Apoapse's Accoutrement.

[**Amanda Vanilla Outfit Override v1.0**]: Overrides Amanda's outfit with her vanilla Venturer outfit.

[**Nightingale Bow Scoped Override v1.0**]: Overrides Nightingale with scoped version for VR. 

[**Enable TAA FX**](https://www.nexusmods.com/skyrimspecialedition/mods/31392?tab=files): Re-enables TAA FX via VR FPS Stabilizer.  Partial parallax support (only minor graphical glitches) with TAA by adding the following line to \VR FPS Stabilizer\SKSE\Plugins\VRFpsStabilizer.ini:
- taa hf 0.5

[**Clear HUD VR v1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/49657?tab=files): Provides an installer that lets you hide certain HUD elements for Skyrim VR based on your personal preference.

[**Vanilla HUD Size for VR**]: Overrides UI with larger vanilla sized HUD.

[**VRIK Rift-Index-WMR Controller Bindings V2.1.0**](https://www.nexusmods.com/skyrimspecialedition/mods/23416?tab=files): These control bindings are an optional add-on for VRIK to make it easier to use holsters.  The button for shout has been moved to Right A (or the right WMR touchpad), and interact is performed by squeezing the right grip.  Sprinting is now done by squeezing the left grip.  With these "safe" inputs on grips, players do not need to worry about shouting accidentally when grabbing holstered weapons.

[**Vanilla Cubemaps for Darker Water**](https://www.nexusmods.com/skyrimspecialedition/mods/30571?tab=files): Optional cubemaps without reflections for darker nighttime water.

[**Equipable Female Tattoo UNP CBBE v1.0**]: Mod adds 5 x Equippable Tattoo skins for UUNP or CBBE Options are: Bijin, Leyenda or Fair Skin Complexion.

[**Replace spiders with wolfs and bears v1.0.1**](https://www.nexusmods.com/enderalspecialedition/mods/31?tab=files): Replaces spiders with wolves and bears.

[**Arachnophobia - No Spiders and Beetles v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/359?tab=files): This mod replaces Spiders with Wolves and Beetles with Bears.

[**Story Mode v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/123?tab=files): Enderal Story Mode includes gameplay tweaks to make the game enjoyable without worrying about micromanaging and difficulty.  Disables EGO when Somnium mods are active.  (eng/ger/rus)

[**Story Mode - No Health Regen v1.01**](https://www.nexusmods.com/enderalspecialedition/mods/123?tab=files): Enderal Story Mode includes gameplay tweaks to make the game enjoyable without worrying about micromanaging and difficulty.  Disables EGO when Somnium mods are active.  (eng/ger/rus)

[**Noble Quarter Player Home Fixes (and EGO patch) v1.0**](https://www.nexusmods.com/enderalspecialedition/mods/409?tab=files): Fixes a small issue with "Enderal - Nobles Quarter Player home redone SE" and ensures compatibility with EGO and other mods.

[**Allow Fast Travel v1.3**](https://www.nexusmods.com/enderalspecialedition/mods/42?tab=files): Allows Fast Travel in Enderal.
- Must be placed near end of load order as any mods that alter worldspace will break fast travel.

[**SSEEdit_Output**]: Conflict resolution patches generated with [**SSEEdit**](https://www.nexusmods.com/enderalspecialedition/mods/78?tab=files).

[**Nemesis_Output**]: SkySA Animations patch generated with [**Nemesis**](https://github.com/ShikyoKira/Project-New-Reign---Nemesis-Main/releases). 

[**xLODGen_Output**]: Terrain LOD patch generated with [**xLODGen**](https://stepmodifications.org/forum/topic/13451-xlodgen-terrain-lod-beta-81-for-fnv-fo3-fo4-fo4vr-tes5-sse-tes5vr-enderal-enderalse/).

[**TexGen_Output**]: LOD textures and billboards patch generated with [**DynDOLOD Standalone 3.0**](https://www.nexusmods.com/skyrimspecialedition/mods/32382?tab=files). 

[**DynDOLOD_Output_PERFORMANCE**]: Object and tree LOD patch generated with [**DynDOLOD Standalone 3.0**](https://www.nexusmods.com/skyrimspecialedition/mods/32382?tab=files). 

[**DynDOLOD_Output_QUALITY**]: Object and tree LOD patch generated with [**DynDOLOD Standalone 3.0**](https://www.nexusmods.com/skyrimspecialedition/mods/32382?tab=files). 

[**Synthesis_Output**]: SkyVRaan patch generated with [**Synthesis**](https://github.com/Mutagen-Modding/Synthesis/releases).

## GAME TWEAKS 
Recommended game settings are listed below.  Note that the above Wabbajack install has already been pre-configured with the following tweaks which are merely listed for reference.

### INI Settings
* INI files are found in C:\ (Your Game Folder)\profiles\Enderal VR Essentials
* These INI files will override any vanilla INI files which are stored in: C:\Users\ (Username)\Documents\My Games\Skyrim VR\  
* Recommended INI settings: 
1. Open skyrimvr.ini and add this text somewhere under the [Launcher] section: bEnableFileSelection=1 (Enables mods)
2. Open skyrimvr.ini and add this text somewhere under the [VR] section: bAllowVRCheating=1 (Disable bumpback when too close to an object)
3. Open skyrimvr.ini and add this text somewhere under the [VR] section: fVrScale=72 (Tweaks world scale for VR; Typical values are between 72-78)
4. Open skyrimvr.ini and add this text somewhere under the [VRUI] section: fHUDCompassScale=0.5000 (Decrease compass size)
5. Open skyrimvr.ini and add this text somewhere under the [VRUI] section: bPlayVRMeleeWorldImpactSounds=0 (Disable impact sounds; Set to "1" if you like the effect.)
6. Open skyrimvr.ini and add this text somewhere under the [VRUI] section to decrease rollover text size: 

         fActivateRolloverSecondaryScale=10	 
         fActivateRolloverSecondaryZ=0	 
         fActivateRolloverSecondaryY=0	 
         fActivateRolloverPrimaryScale=10	 
         fActivateRolloverPrimaryZ=0	 
         fActivateRolloverPrimaryY=0	 
         fActivateRolloverWandScale=10.0000 	 
         fActivateRolloverSecondaryScale=10.0000	 
         fActivateRolloverPrimaryScale=10.0000
	
7.  Open skyrimvr.ini and add this text somewhere under the [VRInput] section to decrease melee sensitivity: 

         fMeleeLinearVelocityThreshold=3.0000	 

8. Open skyrimprefs.ini and add this text somewhere under the [VRWand] section: fBowHoldOffsetY=-6.6 (Tweaks bows for VR)
9. Open skyrimprefs.ini and add this text somewhere under the [Particles] section: iMaxDesired=1500 (Tweaks Embers XD)
10. Open skyrimprefs.ini and add this text somewhere under the [Display] section: bUseTAA = 1 (Fixes menus in Enderal VR; Requires TAA tweaking via VR FPS Stabilizer)
11. Open skyrimprefs.ini and add this text somewhere under the [Display] and [Trees] section: (Recommended tree settings from [STEP guide](https://stepmodifications.org/wiki/Guide:Skyrim_Tree_Settings)): 

         [Display]	 
         fMeshLODLevel1FadeTreeDistance=6144
         fMeshLODLevel2FadeTreeDistance=4096 
         fTreesMidLODSwitchDist=8192	 

         [Trees] 
         bRenderSkinnedTrees=1
         uiMaxSkinnedTreesToRender=200
	
12. Open skyrimprefs.ini and REPLACE all text under the [LOD] and [TerrainManager] section with the following lines for higher performance (**OPTIONAL; Will cause visual pop-in issues.  Only recommended for very low end GPUs**): 

         [LOD]	 
         fLODFadeOutMultObjects=3.0000
         fLODFadeOutMultItems=2.0000
         fLODFadeOutMultActors=2.0000 

         [TerrainManager]
         fBlockLevel0Distance=20000.0000
         fBlockLevel1Distance=42000.0000
         fBlockMaximumDistance=90000.0000
         fSplitDistanceMult=0.750
         fTreeLoadDistance=25600.0000
 
### In-Game Settings
1. Set Movement speed to 50%
2. Activate "Physical Sneaking" and "Realistic Bow Aiming"
3. Disable "FOV Filter when Moving"
4. Set Supersampling slider to minimum (all the way left)
5. Disable Dynamic Resolution
6. Enable Temporal AA (Only enable TAA if applying TAA tweaks via VR FPS Stabilizer)
7. Disable Foliage Shadows
8. Untick “Disable LOD” options and set the Tree Lod slider to max
9. Enable "Skinned trees"
10. Enable "Animated trees"
11. Distance sliders are set to: Item 20%, Actor 20%, Objects 40%, Grass 100% (Skip this step if you adjusted [LOD] values manually in skyrimprefs.ini)

### MCM Settings
* VRIK MCM 
1. Disable "Adjust Held Weapons Position" to fix scoped bow aiming. 
2. Select Body Holsters > Scroll down to Left Shoulder Holster > Untick "Visible".  This prevents your bow from clipping into the edge of your FOV when crouching in real life.

* Spell Wheel VR MCM: 
1. Select Presets > SpellSword + More Pages (Loads preset for equipping spells, weapons, and items from the spell wheel across multiple pages)
2. Select General > Tick "Unequip to Grab with Higgs" (Allows you to grab potions directly from the Spell Wheel menu to your hand for added immersion)
3. Select Advanced > Set "Slow Time Scale" to 5.  (Enables slow motion when selecting items from the spell wheel)

## Nemesis Configuration

### ADXP
ADXP is a framework built on SkySA that bypasses the Skyrim animation wall, allowing for modern combat.  It brings chainable power attacks, animated charged attacks, animated transitions and non linear movesets to Skyrim.  While most of these features are inconsequential in VR as you never see the player moving in third person, ADXP is extremely useful in overhauling NPC animations.  With this mod, enemies move slower with more fluid Dark Souls style movements during combat. ADXP has been pre-configured with Wabbajack but the configuration process has been documented below for reference.   

1. In Windows, navigate to "Virus and Threat Protection" > "Manage Settings" and temporarily untick "Real-time protection" or Windows may prevent Nemesis from running properly.
2. Install "VR Address Library for SKSEVR", "Dynamic Animation Replacer for Skyrim VR", "Animation Motion Revolution VR", and "ADXP" (delete MCO.dll) mods.
3. Download Nemesis Unlimited Behavior Engine from [HERE](https://github.com/ShikyoKira/Project-New-Reign---Nemesis-Main/releases).
4. Launch MO2 and install Nemesis Unlimited Behavior Engine as a regular mod.  (This tool must be run from the MO2 virtual file system or Skyrim Data folder)
5. Select Tools > Executables > Add an executable ("+" icon in upper left) > Add from file > Navigate to "Nemesis Unlimited Behavior Engine.exe" in the \mods\Nemesis\Nemesis_Engine\ subfolder in your MO2 folder and select "Open"
6. Right click on "Overwrite" in the left window pane and select: Clean Overwrite > OK.  (If applicable, this option may not be available if your overwrite older is already clean)
7. Select Nemesis Unlimited Behavior Engine from upper right drop down and click RUN
8. Click OK for both Warning pop-ups
9. Click "Update Engine"
10. Tick the "Attack - Distar Experience" option.
11. Click "Launch Nemesis Behavior Engine". 
12. Wait for the process to finish and then close the Nemesis Unlimited Behavior Engine.  
13. Right click on "Overwrite" and select "Create Mod".  Enter a custom name i.e. Nemesis_Output and click OK.
14. Tick "Nemesis_Output" in the left window pane. 
15. If using XPMSSE, delete dummy plugin "FNIS.esp".
16. Revert the upper right dropdown bar back to "SKSE".
17. Re-enable "Real-time protection" in Windows.
18. You may need to re-run this process if you change your load order.

## DynDOLOD 3 and SkyVRaan Configuration

### xLODGen/TexGen/DynDOLOD  

DynDOLOD is a set of simple tools based on xEdit/xLODGen to automatically create a Skyrim mod based on the load order which adds distant LOD for objects and trees to Skyrim.  DynDOLOD has been pre-configured with Wabbajack but the configuration process has been documented below for reference. 

Note that many DynDOLOD guides on the Web are heavily outdated or are not relevant for patching Enderal VR.  While DynDOLOD is a dynamic patch and thus a bit more complicated to setup versus standard mods, the processs is fairly quick once you understand the general workflow.  The following steps outline everything necessary to setup DynDOLOD with Enderal VR.

#### Quickstart Guide
1. Install Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019
2. Install the following prerequisite mods: SKSE VR, PapyrusUtil VR, DynDOLOD Resources SE 3.0
3. Install landscape texture mods (Noble + Tamrielic + Septentrional recommended) and tree mods (EVT recommended). 
	- If using EVT for trees, make sure ESP is enabled as it is used by DynDOLOD 3.0.  Remove the plugin's "Worldspace" data in xEdit.
	- Disable any billboards that are included in tree mods (found in \data\textures\lodgen\).
4. Install a terrain LOD mod (that corresponds with the lowest texture mod used for terrain) and place it after other Skyrim SE texture mods.  Only used for terrain noise texture.  Remove ALL files except for the \textures\ folder.
5. Finalize load order in Mod Organizer 2.
6. Launch DynDOLOD to check for plugins with worldspace injection errors.
	- If no errors are found, close DynDOLOD. 
	- If DynDOLOD reports a plugin error, remove the plugin if it isn't required or fix the plugin by removing its Cell and/or Worldspace data with xEdit.
7. Use xLODGen to generate terrain LOD meshes and textures into a dedicated output folder and then install as a mod.
8. Use TexGen to generate object LOD textures and tree/grass LOD billboards into a dedicated output folder and then install as a mod.
9. Use DynDOLOD to generate object LOD (includes grass LOD if enabled), tree and optional dynamic LOD into a dedicated output folder and then install as a mod.
10. (Optional) Remove the Enhanced Vanilla Tree .esp file to avoid potential plugin issues.  Then navigate to \Enhanced Vanilla Trees SE-Lush Trees\meshes\landscape\trees\ and remove the SRG_ prefix from all filenames (required if not using plugin). 

#### xLODGen/TexGen/DynDOLOD Configuration 

1.  If you wish to reset your xLODGen/TexGen/DynDOLOD settings to default, remove all files in the following location: C:\Users\ (Username)\AppData\Local\Skyrim VR\
2.  Install [Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019](https://aka.ms/vs/16/release/vc_redist.x64.exe) if you don't already have it installed.
3. Extract [SKSE VR](https://skse.silverlock.org/beta/sksevr_2_00_12.7z) to your Skyrim VR installation folder.  If you have already setup Skyrim VR or Enderal VR, this step has most likely already been completed.
4. Install the following prerequisite mods through Mod Organizer 2 with default settings (place them high in the load order above all texture mods):
	- [SKSE VR](https://skse.silverlock.org/beta/sksevr_2_00_12.7z) (Scripts folder only)
	- [PapyrusUtil VR - Scripting Utility Functions](https://www.nexusmods.com/skyrimspecialedition/mods/13048?tab=files) (Under "Miscellaneous Files")
	- [DynDOLOD Resources SE 3.00](https://www.nexusmods.com/skyrimspecialedition/mods/32382?tab=files) (Under "Miscellaneous Files")
5. Install a terrain LOD mod through Mod Organizer 2 that corresponds with the lowest texture mod for terrain that you have installed.  If using Septentrional Landscapes SE, the [Terrain LOD for Septentrional Landscapes](https://www.nexusmods.com/skyrimspecialedition/mods/39563) mod is recommended.
	- Place this mod BELOW all other Skyrim SE texture mods in your mod load order in the left window pane.
	- Only used for terrain noise texture.  Remove ALL files except for the \textures\ folder.
6. If using [Enhanced Vanilla Trees SE-Lush Trees](https://www.nexusmods.com/skyrimspecialedition/mods/11008?tab=files) (highly recommended), install all default options + Vanilla (i.e., None) + RAT + SFO Snow Pines.  Keep the \DYNDOLOD\ folders as these are used by DynDOLOD 3.0.  Disable any billboards that are included in tree mods (found in \data\textures\lodgen).  Make sure the ESP plugin is enabled and remove the plugin's "Worldspace" data in xEdit.
7. Finalize your MO2 load order.
8. Download [xLODGen](https://stepmodifications.org/forum/topic/13451-xlodgen-terrain-lod-beta-81-for-fnv-fo3-fo4-fo4vr-tes5-sse-tes5vr-enderal-enderalse/) and extract the contents to a new \xLODGen\ directory that is outside of special OS folders like 'Programs Files' or 'Program Files (x86)', Users, Documents, Desktop, Downloads and also not in SteamApps, game or any mod manager folders.
9. Download [DynDOLOD 3.0](https://www.nexusmods.com/skyrimspecialedition/mods/32382?tab=files) and extract the contents to a new \DynDOLOD\ directory that is outside of special OS folders like 'Programs Files' or 'Program Files (x86)', Users, Documents, Desktop, Downloads and also not in SteamApps, game or any mod manager folders.
10. Launch Mod Organizer 2.
	- Select Tools > Executables  
	- Select Add an executable ("+" icon in upper left) > Add from file > Navigate to "xLODGenx64.exe" in the folder created in Step 5 and select "Open" > Type -tes5vr -o:"c:\xLODGen_Output\" under "Arguments" and click "Apply".  
	- Select Add an executable ("+" icon in upper left) > Add from file > Navigate to "TexGenx64.exe" in the folder created in Step 6 and select "Open" > Type -tes5vr under "Arguments" and click "Apply".  
	- Select Add an executable ("+" icon in upper left) > Add from file > Navigate to "DynDOLODx64.exe" in the folder created in Step 6 and select "Open" > Type -tes5vr under "Arguments" and click "Apply".  
	- Click OK to return to the main Mod Organizer 2 window. 
11.  Select DynDOLODx64 from the upper right drop down bar and click Run.  (We are not ready to use DynDOLOD yet but need to run the tool now to check for potential errors in our modlist) 
		- If you receive an "Injected Worldspace" error for a mod which does not require plugins to work (i.e. texture/mesh mods), delete the .esp files associated with the mod.
		- If you receive an "Injected Worldspace" error for a mod which requires plugins to function, fix the .esp files associated with the mod by opening the mods plugins in xEdit and deleting all Cell and Worldspace data.
		- If you receive a "Worldspace Editor ID MQP01 Home is changed to Tamriel" error, you can simply ignore this error. 
		- Close the DynDOLOD window once it appears.
12.  Select xLODGenx64 from the upper right drop down bar and click Run.
		- Untick MQP01Home and tick all other world spaces once the xLODGen window appears.  Tick Terrain LOD.  Set "Optimize Unseen" to 500.  Tick "Protect Borders".  Leave Objects LOD, Trees LOD, and Occlusion unticked.  Then click Generate.	
		- Close the xLODGen window once you see "LOD generation complete".	
12.  Navigate to C:\xLODGen_Output\ and move this folder to C:\ (Your Game Folder)\mods.  Refresh MO2 with "F5" and enable xLODGen_Output in the left window pane.  Place this mod near the end of your load order.
13.  Select TexGenx64 from the upper right drop down bar and click Run.
		- If you get a "Could not open registry key" error, launch vanilla Skyrim VR one time from Steam.  Then exit Skyrim VR and repeat this step.  (This step can be performed outside of VR.  Simply launching Skyrim VR from your flatscreen and exiting after any Steam VR errors regarding no detected headset is sufficient.)
		- If you get a "Found stitched object LOD textures" error, click "Ignore".
		- Tick "HD Trees" and click "Start" once the TexGen window appears.  If you get a "Worldspace Editor ID" error, click "Ignore".
		- Wait for TexGen to finish running, it typically takes several minutes.  When the process completes, click "Exit TexGen".
14.  Navigate to your \DynDOLOD\ folder from Step 9 and move the \TexGen_Output\ folder to C:\ (Your Game Folder)\mods.  Refresh MO2 with "F5" and enable TexGen_Output in the left window pane.  Place this mod directly under "xLODGen_Output".
15.  Select DynDOLODx64 from the upper right drop down bar and click Run.
		- If you get a "Worldspace Editor ID MQP01Home is changed to Tamriel" error, click "Ignore".
		- Once the DynDOLOD window appears, click "Advanced".  Then tick all world spaces minus MQP01Home, click "High" at the top of the window,  tick "Ultra", and tick "Occlusion data" in the options below.  Then click "OK" to start the process.  Wait for DynDOLOD to finish running, it typically takes several minutes.  When the process completes, click "Save & Exit". 
		- Under "Mesh and Reference rules", 'tree' can be set to Level0/Billboard2/Billboard2 under LOD Level 4/8/16 respectively for slightly improved visuals.  Not recommended for VR due to the moderate performance drop.  
16.  Navigate to your \DynDOLOD\ folder from Step 9 and move the \DynDOLOD_Output\ folder to C:\ (Your Game Folder)\mods.  Refresh MO2 with "F5" and enable DynDOLOD_Output in the left window pane. Place this mod directly under "TexGen_Output".
17.  Confirm "xLODGen_Output", "TexGen_Output", and "DynDOLOD_Output" are ticked in the left window pane and ensure DynDOLOD.esp is ticked in the right window pane.
18.  Navigate to \Enhanced Vanilla Trees SE-Lush Trees\ folder and delete the ESP file (untested with Enderal VR), then navigate to \Enhanced Vanilla Trees SE-Lush Trees\meshes\landscape\trees\ and remove the SRG_ prefix from all filenames (required if not using plugin). Then press F5 with the right window pane selected to refresh the active plugin list. You will need to reinstall EVT with its plugin if you ever wish to re-run DynDOLOD.  
		- This step is unnecessary but frees up a slot in your plugin list.
19.  Revert the upper right dropdown bar back to "SKSE".
20.  DynDOLOD is now successfully configured!  You should see FAR more detail in the distance when looking across large open areas of the game! (You may need to re-run this process if you change your load order.)

### SkyVRaan Configuration 
SkyVRaan adds shimmering water effects to the game.  This process should be run immediately before or after xLODGen/TexGen/DynDOLOD (if using xLODGen/TexGen/DynDOLOD). DynDOLOD and SkyVRaan's Synthesis plugin should be placed in your load order in the order that they are generated.  SkyVRaan has been pre-configured with Wabbajack but the configuration process has been documented below for reference.  

1. Download SkyVRaan from [HERE](https://www.nexusmods.com/skyrimspecialedition/mods/30571?tab=files) and install it through MO2 underneath other grass and water mods.  Tick "Rally's Water Foam (4K)" and "Improved Water Normals for Vanilla" and leave all other settings at default.  Do NOT install Rocky Riverbeds due to high performance drop.
2. Recommend replacing 'OutputCube.dds' with 'ewpdefault.dds' from the [Enhanced Wetness and Puddles](https://www.nexusmods.com/skyrimspecialedition/mods/58155?tab=description) mod for improved water reflections.
3. If you have previously used Synthesis, you MUST remove files from older versions by removing the following folder:  C:\Users\ (My Username)\AppData\Local\Temp\Synthesis
4. Close Mod Organizer 2 if open
5. Install .NET SDK 5.0 from [HERE](https://dotnet.microsoft.com/download/dotnet/5.0) and remove any previously installed .NET runtimes.  You can confirm .NET SDK 5.0 is properly installed by running the following from your command prompt:  dotnet --info
6. Download Synthesis from [HERE](https://github.com/Mutagen-Modding/Synthesis/releases/) and extract it to a folder anywhere on your drive called \Synthesis\  
7. Launch MO2 and select Tools > Executables > Add an executable ("+" icon in upper left) > Add from file > Navigate to "Synthesis.exe" in the folder created in Step 5 and select "Open"
8. Right click on "Overwrite" in the left window pane and select: Clean Overwrite > OK. (If applicable, this option may not be available if your overwrite folder is already clean)
9. Select Synthesis from upper right dropdown and click RUN
10. Select Skyrim VR (if prompted).
11. Select Git Repository (2nd icon in upper left) 
12. Search for SkyVRaan and select the "+" icon next to SkyVRaanAutoPatcher and SkyVRaanWeatherPatcher
13. Click RUN icon
14. Wait for the utility to report "Completed" and close Synthesis. 
	- If you get a "Blocking Error", try the following:
		-  Delete any existing Groups and try re-running Synthesis.
		-  Delete any files from C:\Users\ (Username)\AppData\Local\Temp\Synthesis
		-  Make sure you are using the latest version of Synthesis from Github [HERE](https://github.com/Mutagen-Modding/Synthesis/releases)
15. Right click on "Overwrite" and select "Create Mod".  Enter a custom name i.e. Synthesis_Output and click OK.
16. Tick "Synthesis_Output" in the left window pane and make sure "Synthesis.esp" is at the bottom of your Plugin load order and ticked in the right window pane. (Place them directly after "DynDOLOD_Output" and "DynDOLOD.esp" respectively if xLODGen/TexGen/DynDOLOD have already been run.) 
17. Revert the upper right dropdown bar back to "SKSE".
18. You may need to re-run this process if you change your load order.

### Mod Organizer 2 Settings
Required Mod Load Order (left side):
* Enderal SE
* Enderal SE - Update
* Enderal SE - Bug Fixes
* SkyUI
* JContainers VR
* moreHUD VR 
* SkyrimVRTools
* Enderal VR patch
* (everything else; Enderal SE specific mods should be placed near the bottom)
* Nemesis_Output
* xLODGen_Output
* TexGen_Output
* DynDOLOD_Output
* Synthesis_Output

Required Plugins Load Order (right side):
* Enderal Forgotten Stories.esm
* Enderal SE - Bug Fixes.esp
* SkyUI_SE.esp
* AHZmoreHUD.esp
* EnderalVRpatch.esp
* (everything else; Enderal SE specific plugins should be placed near the bottom)
* DynDOLOD.esp (Generated with the DynDOLOD utility and should be placed near the bottom)
* Synthesis.esp (Generated with the Synthesis utility and should be placed beneath DynDOLOD) 

When installing mods, if prompted to extract BSA files, select "No".

## Changelog
See [Changelog](https://github.com/Ashok0/EnderalVREssentials-Nightly/blob/main/CHANGELOG.md)

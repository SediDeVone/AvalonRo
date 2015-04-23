AvalonRO
=======================
AvalonRo (avalonro.net) is the set of scripts made by me for private Ragnaron Online server based on Hercules emulator.

# What is Hercules?
Hercules is a collaborative software development project revolving around the creation of a robust massively multiplayer online role playing game (MMORPG) server package. Written in C, the program is very versatile and provides NPCs, warps and modifications. The project is jointly managed by a group of volunteers located around the world as well as a tremendous community providing QA and support. Hercules is a continuation of the original Athena project. You can find the github page at https://github.com/HerculesWS/Hercules.

Scripts

Easter Egg
---------
	Script is spreading 15 spots all over the server. Each player can interact with each spot only once per day, and the spots last for 7 days, meaning a player can only have a maximum of 15 eggs each day and a total of 105 eggs for the whole duration of event.
	Script is supporting an NPC that jumps from town to town. Players can interact with NPC to covert their eggs into awesome prizes. Once a price is chosen the Fairy is taking a 1 hour break after which she jumps to another city. Once the Fairy jumps the broadcast informs players that the Fairy has moved. 
	Implemented spot locations:
	``` C
	Prontera (27, 161)
	Payon (173, 242)
	Knight_3-1 (82, 82)	
	lhz_dun03 (75, 154)
	thor_v03 (216, 51)
	prt_church (180, 29)
	Umbala (139, 197)
	prt_fild08 (74, 318)
	moc_pryd06 (148, 64)
	ice_dun03 (150, 100)
	louyang (91, 253)
	anthell01 (29, 266)
	gef_tower (119, 22)
	moc_fild18 (48, 204)
	Geffen (173, 98)
	```

EventMap1Wall, KarinChanWall, Regicide Wall and buff_test
---------
	Simple script support custom maps. Game Masters are able to create walls, that are filled with monsters, to prepare for certain events. Once they feel that they are ready, and people participating in the event too, they can remove the walls so the event can start.

Lucy
---------
	Lucy is `adding` missing commands for Game Masters such as: guild recall, recall map, lock guild and unlock guild. The script is using OnWhisperGlobal function which means that people can whisper NPC (NPC:Lucy). It lets GMs recall whole guild to you, recall whole map to you, add or remove mf_guildlock mapflag.

PVPreward and PVPreward_old
---------
	Both scripts do the same thing. They support PvP system on your server. The major difference between this two files is how arrays of items are initalised.
	System supports spectator map, mostly used for PvP events. When player who wants to spectate talks to NPC he is being muted, hiden and costumed (they can't cast spells or speak). Players who wants to spectate can't have homunculus or pets with them. They also can't join while being in party, to prevent party invite spam.
	System supports multiple PvP restrictions such as: General PvP, General PvP without Valkyrie Card, General PvP without High Wizard Card, Fallen Bishop Card or Valkyrie Card or Magic Classes. Game Masters are able to choose the specific map for the event as well.
	The whole system got implemented two item checks. One of them checks if you don't own consumable foods plus the items set in restrictions. All of this is checked while talking to NPC. The second scripts checks every player on event map for resctricted items, if that item is equipped it is being deequipped. 
PVP_Ladder
---------
	PvP Ladder is script that supports ... PvP Ladder. It tracks people's stats, their kills, their deaths, their last victim and their last killer. It has implemented few basic antifarm cheats in case someone would like to trade their kills into goodies. Game Masters above level 99 are able to reset whole ladder.
leviathan
---------
	Leviathan script is role playing script to summon custom MvP Leviathan. NPCs that you have to visit are spread around hugel and geffen. This lovely people will share their ways with you only if you prove worthy, which means that players got to bring certain items with them. Altough the requirements are quite high it is worthy, because who wouldn't want to meet Leviathan itself.
premium_buffer
---------
	Premium buffer is very basic script that supports buffing players with basic buffs for small fee. It also let's players create own list of buffs so they can get all wanted buffs with just one click.
premium_warper
---------
	Premium warper is very basic script that supports warping players to certain places for small fee. 
thana_quest
---------
	It is official Thanatos Tower script with one small modification. Instead of opening portal from tha_t12 to thana_boss, the statues check which player/party inserted the most crystals and only they are warped inside the map. If for some reason the group of people who `won` the race for Thanatos failed in killing either monsters or boss, the script will open the portal at tha_t12 to thana_boss after 5 minutes.

# License
The data provided by WoW Token Info in the links below is made available under the MIT License. You are free to share the data, to produce works from the data, and to modify and build upon the data, as long as you understand and follow the below conditions: 
```
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

## There is no warranty with this service, neither expressed nor implied.
   * This is an unofficial service, provided by a guy with a computer at his house.
   * We may miss engine updates due to the many factors out of our control. The engine upgrade might break script, my cable modem might fail, solar flares...
   * We may need to change the format of the script without warning. Though we'll try not to do that.

If you use data from this website for a public work, we ask that you mention and link to https://github.com/Alvaren/AvalonRo in your work.

If your server has employees, then you probably don't want to rely on this, and should instead get your version of scripts.

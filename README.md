# Project Ignis GX Changes:

Reimplementing the game in order of OCG Release
* Will also include TCG exclusives
* The end of each era will herald in a series of custom and anime/game-exclusive cards
* Dedication to a balanced and interesting sandbox and retroactive Problem Solving Card Text

Mass Renaming
* Cards with generic names given new ones inspired by mythology and folklore
* Cards whose names were poorly translated or censored given more proper translations

General Effect Rebalancing
* Removal comes at a premium: Expect to go -1 off removal effects (including effects that negate and destroy)
* More "Pay LP until you have 100 Left" effects. Effects like Solemn Judgement and Cyber-Stein are now hard-countered by Sparks.
* Stronger healing effects, Dian Cecht the God of Healing for example heals 4000 LP instead of 1000
* Cards now specify whether they target players

Reworked ATK/DEF
* Normal Monsters will always have more ATK and DEF than effect monsters with beneficial effects
* The ATK/DEF of monsters can go up to 10,000, for example, Blue-Eyes White Dragon's ATK/DEF is 4000/3500

Fixed "Missing the Timing" for everything except Counter Traps
* All counter effects use "When... You Can" syntax, every other effect uses "If... You Can" syntax instead

Buffed Weak Types
* Ritual Spells can now Ritual Summon monsters from the Deck
* Toons now all contain the text "This card can attack directly. After damage calculatin, if this card battled: Banish this card."
* Spirit monsters now all contain the text "During the End Phase: Return this card to the hand." and can be Special Summoned.

Reworked Union Monsters
* Effects preceeded by FIELD:, HAND:, MONSTER:, or SPELL/TRAP: can only be activated in the respective locations
* Effects that can only possibly occur in the monster zone like "If this card is Special Summoned:", do not have MONSTER: preceeding them
* "Union Place", short for "place face-up in your Spell/Trap Zone", often followed by "as a Continuous Spell"
* "Union Equip", short for "place this card face-up in your Spell/Trap Zone as an Equip Spell Card and equip", often followed by "to a monster"

Reworked Contact Fusion
* Officially a type of Fusion Summoning, and not just Special Summoning
* Supported by most Fusion Monsters
* Can use materials from your Spell/Trap Zone, unlike Fusion Summoning through card effects

Reworked Types
* Winged Beast merged into Beasts, support will specify WIND Beasts
* Dinosaur merged into Reptiles, fear the day Snake Rain is implemented
* Beast-Warrior split into Warrior and Beast (Did someone at Konami want to add dual types but everyone else say no and this was the compromise?)
* Wyrm merged into Dragons
* Creator God merged into Divine Beast (Creator God is good for lore, not so great for type support)
* Psychic redefined to mean monsters who are heavily associated with using or manipulating brains and logic/or (musicians, psychics, scientists, etc)
* Cyberse merged into Psychic (they are monsters made of data aka logical instructions)
* New Aquatic type, includuds former non-dragon members of Sea Serpents, former non-elemental members of Aqua, and former members of Fish
* New Elemental type, represents monsters that are elements given form, such as ghosts, snowmen, and gnomes (greek mythology is weird) 
* Pyro, Thunder, and the rest of Aqua merged into Elemental (I'm sorry Fire Kraken)
* Removed Tuners, Synchros, Xyz, Pendulums, and Link
* Equip Traps now exist de-jure
* Ritual Traps now exist
* Union monsters now represent monsters which can exist in either the Spell and Trap Zone or the Monster Zone
* Removed Nomi Monsters

# Original Project Ignis EDOPro README contents
# Project Ignis: EDOPro
All assets for the game, except card images. See LICENSE and COPYING in each folder for proper credits, copyright, and rules for redistribution.
On Windows, please do not put your game install in Program Files, Downloads, or any other location that might be read-only or require admin permissions.
On Linux, after moving the game install to your preferred location, you can run `./install.sh` from a terminal to install desktop files for the current user.

## System requirements

Supported platforms:
- Windows 2000 or later, 32-bit or 64-bit
- macOS 10.11 or later
- 64-bit GNU/Linux with X11 and glibc 2.27+ (e.g. Debian 10+, Ubuntu 18.04+, Fedora, CentOS 8+, rolling release distros like Arch)

DirectX 9 or OpenGL 1.0 supporting graphics driver required.

1 GB free disk space recommended for asset updates and images.

1 GB free RAM recommended, though the game is not expected to exceed 300 MB of memory unless you spam the restart button.

### Prerequisites for WindBot Ignite (AI):
- Windows: install .NET Framework 4 if you don't have it. This ships with Windows 10.
- Linux: install the mono-complete package https://www.mono-project.com/download/stable/#download-lin
- macOS: install Mono with the .pkg https://www.mono-project.com/download/stable/#download-mac

## Keyboard and mouse shortcuts

### General:
* ESC: Minimizes the window if not typing
* F9: Reload audio
* F11: Toggles fullscreen
* F12: Captures a screenshot
* CTRL+O: Opens the additional settings window
* R: Reloads fonts if not typing
* CTRL+R: Reloads current skin
* CTRL+1: Switch to card info tab
* CTRL+2: Switch to duel log tab
* CTRL+3: Switch to chat log tab
* CTRL+4: Switch to settings tab
* CTRL+5: Switch to repositories tab
* Drag and drop support for files and text:
	* drop an `ydk` file in the main menu or the deck edit area to load that deck
	* drop a card passcode or card name in the deck edit area to add that card to the deck
	* drop a `ydke://` URL in the deck edit area to load the deck specified by that URL
	* drop a `yrpX` file in the main menu or the replay selection menu to load that replay, if valid
	* drop a Lua file in the main menu or the puzzle selection menu to load that puzzle, if valid
	* drop text in a text box to insert text
	* drop a `.pem`, `.cer`, `.crt` certificate bundle file to make the client use that for ssl verification (if you're getting ssl certificate is invalid)

### Deck editor:
* Right Mouse Button: Adds/removes a card from the deck
* Middle Mouse Button: Adds another copy of a card to the deck or side deck
* Shift+Right Mouse Button or Hold Left Mouse Button then click Right Mouse Button: Adds a card to the side deck
* With the exception of Shift+Right Mouse Button, holding Shift will ignore ALL deck building rules

While not typing:
* CTRL+C: Copies a `ydke://` URL of the deck list for sharing
* CTRL+SHIFT+C: Copies a plain text deck list for sharing
* CTRL+V: Imports a `ydke://` URL decklist from the clipboard

### Duel:
* Hold A or Hold Left Mouse Button: Lets the system stop at every timing.
* Hold S or Hold Right Mouse Button: Lets the system skip every timing.
* Hold D: Lets the system stop at available timing.
* F1 to F4: Shows the cards in your GY, banished, Extra Deck, Xyz Materials respectively.
* F5 to F8: Shows the cards in your opponent's GY, banished, Extra Deck, Xyz Materials respectively.

### macOS:
Note that system hotkeys may intercept some of the above keyboard shortcuts.
The following app shortcuts are also available in the app and dock menus:
* Cmd+N opens a new instance with audio muted
* Cmd+Q quits the game
* Ctrl+Cmd+F toggles fullscreen

## Deck editor search functions
* `string`:
	returns all cards that have `string` in their name OR in the card text.
	Example: `Hero`
* `@string`
	returns all cards that belong to the `string`  archetype.
	Example: `@Hero`
* `$string`
	returns all cards that have `string` in their name only, which ignores the card text.
	Example: `$Heroic`
* `string1||string2`
	returns all cards that have `string1` OR `string2` in their name/text.
	Example: `Trickstar||Bounzer`
* `!!string`:
	negative lookup (NOT)
* `string1*string2`
	replaces any character in any amount. Example: `Eyes*Dragon` will return cards Blue-Eyes White Dragon, Red-Eyes B. Dragon, Galaxy-Eyes Photon Dragon, etc.

These can be combined. Example: `@blue-eyes||$eyes of blue` returns all cards that belong to either the `Blue-Eyes` archetype or have `Eyes of Blue` in their names.

The ATK, DEF, Level/Rank, and Scale textboxes support searching for `?`. You can also prefix the search with comparison modifiers <, <=, >=, >, and =. 

## Test hand
A Hand Test mode is accessible from the deck editor, with quick restart.
The duel will never end normally in this game mode (e.g. running out of LP, decking out)
* From version 38.1.4 onwards it is also possible to change the ammount of cards in the initial hand, number of cards per draw, disable deck shuffle or even give the opponent a copy of your deck (for interactions like One Day of Peace).
	* Notice that this mode was not made to control the opponent. Dueling vs yourself in LAN Mode would be a better option for that.

## Discord Rich Presence
Works with the desktop version of Discord. In your Discord settings, turn on Game Activity first.

Your status on Discord will update to be playing a game, including elapsed time.
Activities displayed in Rich Presence:
* Dueling
* In menu
* Playing a puzzle
* Watching a replay
* Editing a deck

### Game invites
Host a room on a server (LAN does not work). In the appropriate channel or private message, the upload (+) icon should change to have an additional green play button.
Clicking on it will send out a game invite to your room with your message of choice. If the room is locked, the password will be skipped for invitees.
Users can accept the invite while EDOPro is closed if they've started it once before; the game should be launched automatically. Note that Discord is rather fickle and changes this behaviour on us very frequently, so if the game fails to automatically launch, try starting the game.

## Customization

### Default textures:
See README in `textures`.

### Skins:
Editable by adding subfolders to **skin**. For each folder, provide a unique `skin.xml` file, with the changes you want.
You can switch skins in the settings (CTRL+O). For instructions on the supported fields and what they change, see README in `skin`.

### Audio:
See README in `sound`. There are many new features, including summon chants!
Music and sound volume controls are also separated.

### MSAA (antialiasing)
Makes sharp/pixelated edges softer, but requires more performance.
2D elements might look blurred at higher levels. Rendering results are hardware- and device-dependent.
The program will automatically try smaller MSAA values if the driver does not support the specified MSAA level.

## Advanced configuration

### system.conf
`config/system.conf` handles most of the configurations available in the game. It is overwritten when the game is closed normally.
Only options not directly configurable in-game are listed here.
Configurations listed as "boolean" accept either 0 for 'disabled' or 1 for 'enabled'.

| Name     | Purpose | Example |
| -------- | ------- | ------- |
| use_d3d  | Windows-only. 1 = Direct3D 9; 0 = OpenGL 4.  | |
| textfont | path to the font used for texts and its size | fonts/NotoSansJP-Regular.otf 14 |
| numfont  | path to the font used for numbers            | fonts/NotoSansJP-Regular.otf |

If a character cannot be found in the supplied font, it will not be displayed. The shipped font supports all characters that appear on Yu-Gi-Oh! cards in Latin alphabets and Japanese.

### configs.json
`config/configs.json` handles the servers the client is connected to, which include repositories for updates, servers for duels and pictures.

#### repos (array)
* url: required, the complete url of the repository to check for updates.
* repo_path: optional, the subdirectory in the client's directory where the contents will be saved. If not provided, the folder will be created in the expansions folder and will have the repository's name.
* has_core: optional.
* core_path: optional, used if has_core is true.
* data_path: optional, the folder where the databases and the strings will be loaded from in the repository. If not provided, it will load from the main folder of the repository.
* script_path: optional, the folder where the scripts will be loaded from in the repository. If not provided, it will load from the script folder of the repository.
* pics_path: optional, the folder where the pics will be loaded from in the repository. If not provided, it will load from the pics folder of the repository.
* lflist_path: optional, the path for lflists, if the repository contains any.
* should_update: true/false, optional, if the client will download the contents of the repository. If the repository is missing, it will still be downloaded only for the first time. If not provided, it will be set to true.
* should_read: true/false, if set to false the game will ignore that repository. If not provided, it will be set to true.

#### urls (array)
* url: A URL format string for direct card image download, or "default". Should contain `{}` to be replaced by the client with the card's passcode.
* type: pic/field/cover

#### servers (array)
* name: Display name
* address: URL (domain or IP works) for connecting to rooms nad hosting
* duelport: port for the above
* roomaddress: URL for retrieving the room list via the REST API
* roomlistport: port for the above

#### posixPathExtension
Used on macOS and Linux as additional search paths for Mono, required to run WindBot Ignite. Generally you should not need to change this.

## Miscellaneous differences from YGOPro Percy 1.034 Links Beta

#### New TCG/OCG and anime cards by:

* aht
* AlphaKretin
* andré
* Cybercatman
* edo9300
* Eerie Code
* Hatter
* Hel
* Larry126
* Logical Nonsense
* Naim
* pyrQ

### Client

* Localhost AI added with up to four bots per duel in the first four player slots.
	* Uses custom WindBot Ignite.
	* 27 AI decks (33 from version 38.1.0 onwards).
	* Bots incompatible with the Master Rule used in the room are not displayed.
	* Decks used by Windbot do not necessarily match the current banlist: they follow the OCG banlist available when they were implemented.
		* To avoid warning regarding banned cards, the "Don't Check the Deck" option is suggested.
	* To duel the bot: LAN + AI ->  Host -> OK -> Local AI -> Add AI Player
	* List of decks Windbot has access to:
		* ABC-Dragon Buster (from version 38.1.0 onwards)
		* Altergeist
		* Blue-Eyes
		* Blue-Eyes Ritual
		* Burn
		* Chain Burn
		* Cyberse
		* Dark Magician
		* Dragma (from version 38.1.0 onwards)
		* Dragunity
		* Dragun of Red-Eyes
		* Frog
		* Gren Maju Stun
		* Horus
		* Lightsworn Shaddoll Dino
		* Mathmech (from version 38.1.0 onwards)
		* Normal Monster Mash
		* Normal Monster Mash II
		* Orcust
		* Qliphort
		* R5NK
		* Rainbow
		* Rose Scrap Synchro
		* Salamangreat
		* Sky Striker
		* Time Thief (from version 38.1.0 onwards)
		* Toadally Awesome
		* Trickstar
		* Windwitch Gusto (from version 38.1.0 onwards)
		* Witchcrafter Grass (from version 38.1.0 onwards)
		* Yosenju
		* ZEXAL Weapon
		* Zoodiac
	* Known bugs:
		* The AI is not smart, misplaying a lot, which include but is not limited to negating its own monsters, targetting the same cards with removal effects, attacking monsters with higher ATK, etc.
		* Some actions that require selection, like Advanced Ritual Art, might cause the AI to hang on forever.

* Replaced old replay recording system:
	* current system is now unaffected by script changes from when the replay was recorded to when it is played.
	* kept compatibility with the old replay system.
		* old replay mode plays the replay while running the scripts. Use this if you are debugging a card.
	* replays are still subjected to changes in the database entry for a card: if the ID/passcode of a card in the played replay was changed, the replay will still be played without errors, but no description and details for that card will be displayed. If you don't have a picture with that old ID/passcode, it will not be displayed.
	* replays now show the number of turns in the duel.

* Added the option to export the decks used in a replay.
	* decks will be stored in the default deck folder and will be named after the players in the replay.

* Updated handling for live updates:
	* repositories can now be connected, disconnected, enabled or disabled via json file, `/config/configs.json`.
	* different repositories now display their Update Logs separately.
		* the update log now only shows the changes applied after the current instance of the game was initialized.
			* use the "Show Full History" option to see old entries in the log.

* Added an option to rename a deck in Deck Edit, without the user needing to edit the file directly
	* added a mechanism to prevent the usage of characters not allowed in file names.

* Added a "Quick Animation" option

* Added option to set maximum FPS in the configuration file.

* Added back automatic download of arts for Field Spell cards.

* Added the following new settings:
	* independent volume controls for music and sound effects.
	* hide/show archetype names.
	* hide passcodes and scopes. Passcodes are the unique number each card has. Scopes are the region where the card is available and/or its origin.
	* Draw Field Spell arts on the field.
	* show FPS.
	* enable fullscreen.
	* fit the background.
	* accurate resize for backgrounds.
	* scale
		* the "Apply and restart" applies the GUI scale without resizing. Do not spam this button because it will leak memory until the game is properly restarted.
	* skin selection, via dropdown menu.
		* reload skin, that applies the changes to the current skin file without a restart.

* Added shortcut for in game fullscreen toggle [F11]

* Added shortcut for in game access to the additional settings [CTRL + O]

* Updated skins handling.
	* 10 sample skins and a template are provided.
	* skins can now be applied with the game running, without restarting.
	* skins will also support a `textures` folder to make those items more customizable.
	* more details available in the README in your `skin` folder. 

* Changed "Show anime cards" option to "Show unofficial cards", as other types of cards are present.

* "single" folder renamed to "puzzle"
	* updated puzzles that were unsolvable to use pre-errata cards.

* Puzzles can now display a message while in the puzzle selection screen, in the "Puzzle Mode" menu:
	* messages are added with the following syntax:
	```lua
		--[[message
		insert the text here
		]]
	```
* Puzzles now have a "Restart" option.

* Puzzles now can generate a replay.

* Added a "Puzzle Creator" puzzle.
	* Use this to generate a puzzle by declaring a card and a location to place it. When finished, the resulting puzzle is exported.

* "Puzzle Mode" menu now reads subdirectories in the `puzzle` folder.

* "Watch Replay" menu now reads subdirectories in the `replay` folder.

* Forbidden/Limited lists  now are kept in the `/lflists` directory:
	* multiple files are supported, each containing any number of lists.
	* Forbidden/Limited lists now will be read from a `lflists` folder inside of any repository connected.

* Forbidden/Limited lists now can be done by whitelisting:
	* adding `$whitelist` to a list will automatically ban all the entries not set in that list

* Aliasing is now disabled in deck edit.

* Added support for **GOAT Format**:
	* added 2005.4 Forbidden/Limited List, credits to EerieCode, Tungnon and Naim for preparing the file.

* Fixed the dimensions of `field.png`, the picture used for MR1 and MR2 duels. Credits to GK#3620, on Discord.

* Added asynchronous loading system for card images.

* The last banlist used is now remembered after leaving deck edit, a duel, or the client.

* macOS
	* Shift+Right Click to add to side deck in Deck Edit now works like on Windows and Linux
	* Known bug: invoking the binary from the Terminal directly (./EDOPro.app/Contents/MacOS/EDOPro) will never start the game in fullscreen, but no user should be starting the game this way anyway.

* Scripts now load from one subdirectory level in the script folder only.

* Prereleases are supported. Use the 0x100 OT bit.
	* Prereleases appear by default in deck edit and can be specifically filtered for
	* Prereleases can be permitted in duels in addition to "OCG/TCG" mode.
		* Setting the Allowed Card list to TCG allows only cards that are released in TCG.
		* Setting the Allowed Card list to OCG allows only cards that are released in OCG.
		* Setting the Allowed Card list to TCG/OCG allows only cards that are released both in TCG and OCG but not pre-releases.
		* Setting the Allowed Card list to Pre-release allows only cards that are released both in TCG and OCG.
		* Setting the Allowed Card list to Anything goes allows any cards that are released in either TCG or OCG.
	* All card scopes are now listed in card search with the exception of "OCG/TCG", using sysstrings

* Updated many strings called with dialogue boxes and activation prompts used by the client.
	* Update incorrect strings called in the Damage Step
	* All the strings used in the client are now controlled by the `strings.conf` file, being editable, which allows translations for all these elements.

* Added support for translations.
	* inside the `config/languages` folder, add a folder for your language and add a `strings.conf` file there, with the strings translated to your desired language.
	* Check each strings.conf file for translation credits
	* cards.cdb in each of these folders will also be loaded to replace card text in that locale

* Added support for TCG Speed Duel Skills
	* To use a Skill during a duel, add it to the deck first.
		* When the duel starts, the Skill is removed.
		* For Skills that require a specific activation timing you will get a prompt, for others you use the resolution circle above the area where the Skill is displayed.
	* At the moment, Skills are not limited to Speed Duels.
	* Only TCG Skills are available. Duel Link Skills and Skills from Yu-Gi-Oh! VRAINS are not planned at the moment.
	* Important:
		* Do not use Skills in a Tag Duel. Skills in this duel mode are not supported due to core limitations.
		* Do not add more than 1 Skill in the Main Deck, as there is no handling for it.

* Added support for Link Spells ("Judgment Arrows")

* Added support for an arbitrary number of cards in a deck (main, side, extra.)
	* requires editing the deck file, might be tied with the server.
	* the deck displayed in Deck Edit will no longer display a maximum of 60 cards in the main deck if the deck file contains more than that.

* Text can now be copied (CTRL+C) from the chat/duel log.



### Core, Scripts and functions and other

#### OCGCORE: updated from 1.034 standard to edo9300's 7.0

* Updated mandatory trigger effects handling.

* Added support for **Flash Charge Dragon**:
	* updated old scripts of cards with effects that Summon or put themselves on the opponent's field.

* Added support for **Mischief of the Time Goddess**

* Added `Duel.LinkSummon`, which removes the workarounds used for the "Unchained" monsters.

* Removed complex handling of Continuous Traps for when it is possible to activate the card AND its effect in the same chain link

* The following functions have been renamed:
	* `Card.IsLinkState` -> `Card.IsLinked`
	* `Card.IsExtraLinkState` -> `Card.IsExtraLinked` (this one also no longer requires the workarounds that were once used)
	* `Card.IsAttackable` -> `Card.CanAttack`
	* `Card.IsChainAttackable` -> `Card.CanChainAttack`

* Added suport to load other files from within a script (Duel.LoadScript)

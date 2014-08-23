# SpellShop_UI


##### About

A custom UI module for use by map makers, made by zed (alter ego of Selena Gomez)

##### Features

* Buying spells
  * Using gold
  * Using skillpoints (can buy/sell skillpoints)
  * Using both gold and skillpoints
* Selling spells
* Showing info
  * About the spellshop, or about your mod, or you can even write a novel so people have something to do while respawning
* Custom icons

##### Usage

* Put the files in their correct folders
* It's not necessary to edit the .swf, but feel free to do so (source is included in "src SpellShopUI" folder)
* Check and edit the files in "scripts/spell_shop_ui/"
* **Check and edit LUA files in "scripts/vscripts/spell_shop_ui.lua"**
  * I'm no Lua coder, so I called the SpellShopUI:InitGameMode(); from within addon_game_mode.lua
  * **The spells don't work as it is! You have to precache stuff or do something else within LUA - I don't know, it's up to you.**
* Put your custom icons (128 x 128) in "resource/flash3/images/spellicons/", PNG format

###### Events

* Located in custom_events.txt, most are self explanatory
* I didn't list all of them here

```
"spell_shop_ui_toggle_state"
	{
		"player_ID"		"short"
	}
// toggle the _canOpen stat of the shop (if true changes to false, if false changes to true)

"spell_shop_ui_shop_open"
	{
		"player_ID"		"short"
	}
// force the shop open (for example, when entering the trigger area or something. state must allow it)
// "spell_shop_ui_shop_close" is the same but for forcing close

"spell_shop_ui_change_limit"
	{
		"player_ID"		"short"
		"_limit"		"short"
	}
// "_limit" is the number of different spells/abilities a player can own
```

###### Contact

zed` or zed`` on #dota2mods @ irc.gamesurge.net
reddit.com/u/SelenaGomez_
spellshopui@gmail.com

###### Donation

* If you want to donate, I would be more than grateful! 

bitcoin: 1M7E87NXXEpVf3vi4FfGqBSp2e5SbgV1jG
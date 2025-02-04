# VORP Core FAQ

A list of things commonly asked/answered about VORP Core.

__VORP Frequently Asked Questions__

## How can I translate VORP Scripts?
You can choose your own language from the `translation.lua`, `language.lua`, `config.lua` files in VORP Scripts, if you have one, or you can translate your scripts into your own language from the same places.

## How can I translate item name/label/description?
You can edit in `items` table in database (It is not recommended to change the names in the `item` column in `items` table)

## How can I give item/weapon/job?
You can do in `vorp_admin` or you can use command; `/additems <player_id> <item_name> <item_count>`, `/addweapon <player_id> <Weapon_Hash>`, `/addjob <player_id> <job> <job_grade> <job_label>`

## How can I add new items?
`items` table in database

## How can I add images for items in the inventory?
You can add any `.png` image to `\resources\[VORP]\[vorp_essentials]\vorp_inventory\html\img\items` location with the name of the item in `items` table in the database

## How do I add food and drinks?
In the `vorp_metabolism/config.lua` file, you can add any food, drink or health item you want by looking at the other examples. (Don't forget to add the items you add here to the `item` table in the database)

## How can I turn off the huds that appear on the top right (Cash, Gold, ID etc.)?
You can set true `HideMoney`, `HideGold` in `\resources\[VORP]\[vorp_essentials]\vorp_core\config\config.lua`

## How do I prevent everyone from creating 5 characters?
You can set the `MaxCharacters` value in `\resources\[VORP]\[vorp_essentials]\vorp_core\config\config.lua`

## How can I set the amount of time the player has to wait before respawning?
You can set the `RespawnKeyTime` value in `\resources\[VORP]\[vorp_essentials]\vorp_core\config\config.lua`

## How can I add admin to the server?
You can add admin to your server based on the examples in `server.cfg`, `vorp_admin/vorp_perms.cfg` files. In addition, you need to change the content of the `group` column in the `characters` and `users` tables in the database to `admin`

## How can I edit the character height/scale?
`scale` in `skinPlayer` in `characters` table in database

## How can I CK character?
The easiest way is to go to your database, SHIFT+CTRL+F, paste the player's Steam Hex in the search field and delete the results to CK them.

## How do I change the time/weather?
`/time` command or you can use `/weatherui` command to open time/weather management menu

## How can I integrate Discord Rich Presence
After creating an application from the [Discord Developer Portal](https://discord.com/developers), you need to upload assets to the application and fill in the required fields(`\resources\[VORP]\[vorp_essentials]\vorp_core\config\config.lua`) according to the application information

## How can I solve 32 player problem?
Since this problem is caused by CFX, there is no way to solve it outside of CFX. (Bucket/Instance scripts are not very recommended)

### For general RedM problem [RedM FAQ](https://github.com/Z-eus/RedM-FAQ)

### For Support and more [VORP Core Official Discord Server](https://discord.gg/JjNYMnDKMf)
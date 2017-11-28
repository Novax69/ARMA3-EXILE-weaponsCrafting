# weaponsCrafting
Allow peoples to craft weapons in Exile

It allows everyone to craft weapons on Exile servers,

It just places all the crafts on the floor instead of placing them in a Backpack 



How to install ?


If you use CDAH :

go to CDAH_crafting/logic and replace the file CDAH_ExileClient_object_item_craft.sqf with the one given

Copy the folder Custom in your Mission folder.

Open config.cpp, search for class CfgCraftingRecipes

and add below : 

        #include "Custom\weaponsCraft\Crafts\meleeCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\accessoriesCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\ammoCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\itemsCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\launchersCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\pistolsCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\riflesCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\SMGCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\heavygunCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\sniperCrafts.hpp"
       
And it's done ! 


If you don't use CDAH :

Copy the folder Custom inside your Missions folder
Open the config.cpp and search for class CfgExileCustomCode 

Add this line :     ExileClient_object_item_craft = "Custom\Crafts\ExileClient_object_item_craft.sqf";

Then search for class CfgCraftingRecipes and add : 

        #include "Custom\weaponsCraft\Crafts\meleeCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\accessoriesCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\ammoCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\itemsCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\launchersCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\pistolsCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\riflesCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\SMGCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\heavygunCrafts.hpp"
        #include "Custom\weaponsCraft\Crafts\sniperCrafts.hpp"


You then just have to go into the folder Custom/Crafts and edit the files to place your differents craftings inside !

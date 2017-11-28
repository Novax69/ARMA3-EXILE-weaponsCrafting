# weaponsCrafting
Allow peoples to craft weapons in Exile

It allows everyone to craft weapons on Exile servers,

It just places all the crafts on the floor instead of placing them in a Backpack 



How to install ?


If you use CDAH :

1- go to CDAH_crafting/logic and replace the file CDAH_ExileClient_object_item_craft.sqf with the one given

2- Copy the folder Custom in your Mission folder.

3- Open config.cpp, search for class CfgCraftingRecipes

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
       
4- Search for class CfgExileCustomCode and add :

         ExileClient_util_item_getCraftingRecipes = "Custom\weaponsCraft\data\ExileClient_util_item_getCraftingRecipes.sqf";

And it's done ! 


If you don't use CDAH :

1- Copy the folder Custom inside your Missions folder
2- Open the config.cpp and search for class CfgExileCustomCode and add :

      ExileClient_object_item_craft = "Custom\weaponsCrafts\data\ExileClient_object_item_craft.sqf";
      ExileClient_util_item_getCraftingRecipes = "Custom\weaponsCraft\data\ExileClient_util_item_getCraftingRecipes.sqf";
      
3- Then search for class CfgCraftingRecipes and add : 

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

4- It's Done ! Enjoy

         
You then just have to go into the folder Custom/weaponsCraft/Crafts and edit the files to place your differents craftings inside !

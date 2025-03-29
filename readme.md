
# Thermal Katana

A custom katana weapon for fivem!

# Installation

- Put the `ThermalKatana` into your `resources` folder.
- ensure ThermalKatana - add this line in your `server.cfg`

# If using ox_inventory

- Place in `ox_inventory/data/weapons.lua`
```lua
    ['WEAPON_THERMALKATANA'] 			= { label = 'THERMAL KATANA', 		    weight = 1000,	durability = 0.0,	},      		
```

# If using QBCore & qb-inventory

- Place in `qb-core/shared/items.lua`
```lua
['weapon_thermalkatana'] 				 = {['name'] = 'weapon_thermalkatana', 	 		  	['label'] = 'Thermal Katana', 					['weight'] = 13000, 	['type'] = 'weapon', 	['ammotype'] = nil,						['image'] = 'thermalkatana.png', 							['unique'] = true, 		['useable'] = false,["created"] = nil,	['description'] = 'A flame embedded katana filled with the fires from the hell !'},
```
- Drop the next code in `qb-core/shared/weapons.lua`
```lua
['weapon_thermalkatana'] 				 = {['name'] = 'weapon_thermalkatana', 			['label'] = 'thermalKatana', 				['ammotype'] = nil,	['damagereason'] = 'Knifed / Stabbed / Eviscerated'},
```
- Drop the next code in `qb-weapons/config.lua`
```lua
    ['weapon_katana'] 	             = 0.15,
```
# Add the next code to your `BackItems.lua` [devyn-backitems](https://github.com/devin-monro/devyn-backitems) script (OPTIONAL)
```lua
    ["weapon_thermalkatana"] = {
        model="w_me_machette_lr",
        back_bone = 24818,
        x = -0.2,
        y = -0.15,
        z = 0.12,
        x_rotation = 0.0,
        y_rotation = -120.0,
        z_rotation = 180.0,
    },
```
# Credits
- [bobodori](https://www.gta5-mods.com/users/bobodori) 
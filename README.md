# Rebalanced-Deep-Storage
 Patch Blanacing Mod for LWM's Deep Storage's compatible mods.

## What is this?
This is a mod that balances the different available storage mods that use LWM's Deep Storage's storage system.

## What mods are supported?

### Storage Mods
Mods that use the LWM's Deep Storage's system.
- [Primitive Storage](https://steamcommunity.com/sharedfiles/filedetails/?id=2249071438)
- [Simple Storage](https://steamcommunity.com/sharedfiles/filedetails/?id=1961098970)
- [Simple Storage - Refrigeration](https://steamcommunity.com/sharedfiles/filedetails/?id=2029207212)
- [Little Storage 2](https://steamcommunity.com/sharedfiles/filedetails/?id=2166580060)
- [DocWorld](https://steamcommunity.com/sharedfiles/filedetails/?id=1568744597) + [Vanilla Furniture Expanded - Props and Decor](https://steamcommunity.com/sharedfiles/filedetails/?id=2102143149)

### Other Mods
Mods that are given special filter rules, modify balance or are allow special buildings.
Note: If a mod is not here, doesn't mean that it is not supported. Most mods don't require special rules or rebalancing.
- [Dubs Bad Hygiene](https://steamcommunity.com/sharedfiles/filedetails/?id=836308268)
- [Fertile Fields [1.1]](https://steamcommunity.com/sharedfiles/filedetails/?id=2012735237)
- [Concrete For Fertile Fields](https://steamcommunity.com/sharedfiles/filedetails/?id=2035462091)
- [Vanilla Furniture Expanded - Art](https://steamcommunity.com/sharedfiles/filedetails/?id=1968134023)
- [Vanilla Brewing Expanded](https://steamcommunity.com/sharedfiles/filedetails/?id=2186560858)
- [Vanilla Brewing Expanded - Coffee and Teas](https://steamcommunity.com/sharedfiles/filedetails/?id=2275449762)
- [Vanilla Books Expanded](https://steamcommunity.com/sharedfiles/filedetails/?id=2193152410)
- [Rimefeller](https://steamcommunity.com/sharedfiles/filedetails/?id=1321849735)
- [Combat Extended](https://steamcommunity.com/sharedfiles/filedetails/?id=1631756268)
- [Yayo's Combat 3](https://steamcommunity.com/sharedfiles/filedetails/?id=2038409475)

## How was the balancing done?
My idea was to balance around LWM's Deep Storage original balance. The original author put close attention on balancing details, but most mods ignored this and added highly unbalanced stuff, like a shelf capable of holding thousands of stacks with no delay. While it is possible to rebalance those mods to your liking ingame, thanks to Little White Mouse's excellent work, it was really tedious and often things would be overlooked.

In order to assure a fair balance, I created categories for which all the storage buildings must fall. Specific buildings will have more than one category, but they will always have at least one.

### Storage Categories

The categories are as follows:

- General: Stores anything, but will be often limited in amount and mass. - Big (vanilla) shelves and boxes go here.
- Food: Stores food.
  - Meals: Prepared food - Meal tray.
  - Vegetables: Stores vegetarian food.
  - Corpses: Stores corpses. - Meat Hook
- Loose: Stores items that are tiny per piece and normally used in bulk. - Usually these storages will benefit from not having variety in it.
  - Soft Loose: Dry and Light items like plant matter and kibble - This one is for Hampers and bags.
  - Hard Loose: Humid or Hard items like gold and (modded) compost. Includes soft loose. - This one is for things like pots.
  - Heavy Loose: Heavy items mostly, like gold and jade. These will not include soft loose necessarely. - This one is for things like metal barrels.
- Small items: items that are tiny per piece and not necessarely used in bulk. Food and drugs go here. - This is for small shelves.
- Medical: Medicine and drugs. - This one is for specialized buildings like the medicine cabinet.
- Big items: stone blocks, steel, plasteel. Etc.. These go in pallets.
- Toosable items: Anything that goes into a skip goes here too.
- Apparel: Stores Apparel.
  - Armor: Stores Armor Apparel.
- Weapons: Stores weapons.
- Piles: Stores only one kind of item but in great quantities.
- Drinkable items: Beer and modded drinks. - This one is for wooden barrels
- Chemicals: Chemfuel and modded chemicals. - This one is for tanks.

Modded categories:
- (Vanilla Books Expanded) Papers: Books, newspapers and blueprints - This one is for bookshelves
- (Combat Extended OR Yayo's Combat 3) Ammo: Ammunition, make sure it doesn't catch fire.

As you can see, it is quite extensive. I added more stuff as I realized that I was facing a different type of storage.

### Research

At start I didn't want to add research projects, but I quickly realized that I needed to balance the progression of the storage buildings. It just doesn't make sense for 95% of the storage solutions to unlock when "Complex Furniture" got reserached.

I decided to add 7 research projects of different costs. They are as follow
´´´
Neolithic               Medieval                Industrial
Neolithic Storage   -> Medieval Storage ->  Modern Storage.
                    -> Storage Boxes ->     Cardboard Storage
                                            Industrial Storage
                                            Pallets
´´´

All of the industrial level storage requires Complex Furniture as well.



Fertile Field Resources - All of these are loose stuff that would not go well with a pallet. To not spam 'thingDefs' in the filters I decided to place them inside their own thingCategoryDef, located inside Raw Resources.

Supported Mods
Storage Mods
    DocWorld + Vanilla Furniture Expanded - Props and Decor
    Primitive Storage
    Simple Storage
    Simple Storage - Refrigeration
    Little Storage 2
Other Mods (If it is not here, it may be unecessary to patch them. But do say if something seems off.)
    Dubs Bad Hygiene
    Fertile Fields [1.1]
    Concrete for Fertile Fields
    Vanilla Furniture Expanded Art
    Vanilla Brewing Expanded
    Vanilla Brewing Expanded - Coffees and Teas
    Vanilla Books Expanded
    Rimfeller
    Combat Extended
    Yayo's Combat 3

New Research Projects
Neolithic Storage - Things like baskets and pots.
Medieval Storage - Chests, simple shelves and simple racks. Requires Neolithic Storage research.
Modern Storage - Complex shelves and cabinets. Requires Medieval Storage and Complex Furniture research.
Industrial Storage - Expensive and big storage solutions. Requires Smithing and Complex Furniture research.
Pallets - Everything that is on top of a pallet or just a pallet. It requires Complex Furniture research.
Cardboard Storage - Cheaper and faster to use boxes, but also weaker. It also allows the use of storage that uses small cardboard boxes. Requires Complex Furniture research.

Used Vanilla Research Projects
Stonecutting for Pit, Pots and Granary, becuase they require bricks to be built.
Complex Clothing for Bundles Wraps.
Beer brewing for wooden barrels.
Smithing for Skip

LWM's Deep Storage Changes (Mostly research and mod support)

Food Basket is still a raw food storage but now requires Neolithic Storage research.
Skip is a toosable storage now requires smithing research.
Double Shelf is still a general purpose storage but now requires Medieval storage research.
Hayloft is technically a pile type of storage (for hay) and now requires Medieval storage research.
Clothing Rack is still an apparel storage but now require Medieval Storage research.
Meal Tray is still a meal storage and now requires Modern Storage research.
Weapons Cabinet is still a weapon storage but now requires Modern Storage research.
Hampers are now a soft loose type of storage and now requires Modern Storage research.
Medicine Cabinet is a medical type of storage and now requires Modern Storage research.
Tall Shelf is still a general purpose storage but now require Modern Storage research.
Pallet is a pallet type of storage and now requires pallets research.
Covered Pallet is a pallet and soft loose type of storage and now requires Pallets and Complex Clothing research.

Little Storage Changes are the same as their bigger counterparts

Small Food Basket is still a raw food storage but now requires Neolithic Storage research.
Small Double Shelf is still a general purpose storage but now requires Medieval storage research.
Small Meal Tray Rack and Small Hampers now require Modern Storage research.
Small Hampers are now a soft loose type of storage and now requires Modern Storage research.

Primitive Storage Changes

Storage Tent now stores 18 stacks of any kind (2 per tile). It costs 100 wood, 50 steel and 120 textiles to build. It now requires Neolithic Storage research.
Stone Pots now stores 3 stacks of loose items. It is faster to use if it only stores one kind of Item. It costs 30 blocks to build. It now requires Stonecutting and Neolithic Storage research. If Vanilla Furniture Expanded - Art is present, it will require Pottery research instead of Neolithic Storage.
Pits now stores 5 stacks of any kind. It is slow to build and use. It costs 40 wood, 60 steel and 150 bricks to build. It now requires Stonecutting and Neolithic Storage research.
Granary now stores 42 stacks of vegetable items (7 per tile). It is slow to use and build. It costs 50 Hay, 15 wood and 75 bricks to build. It now requires Stonecutting and Neolithic Storage research.
Woven Baskets now stores 5 pieces of apparel with a total weight of 1.5kg. It now requires Neolithic Storage research.
Woodpile now stores 9 stacks of wood (3 per tile). It costs 75 wood to build.

DocWorld Changes

Brick piles now stores 3 stacks of bricks. It costs 50 blocks to build. It is faster to use if only stores one kind of item. It now requires Stonecutting research.
Large Wooden logs now store 9 stacks of wood (3 per tile). It costs 75 wooden logs to build. It doesn't require research to build anymore.
Wooden logs nos store 3 stacks of wood. It costs 30 wood logs to build. It doesn't require research to build anymore.
Wooden Chest now stores 2 stacks of general items. It is faster to use with less variety. It costs 40 wood logs. It now requires Medieval Storage research.
Large Wooden Chest now stores 4 stacks of general items (2 per tile). It is faster to use with less variety. It costs 80 wood logs. It now requires Medieval Storage research.
Armor Stands now store 5 pieces of armor with a total mass of 30kg. It costs 40 wood logs to build. It now requires Medieval Storage research.
Weapon Racks now store 8 weapons (4 per tile) with a total mass of 30kg (15kg per tile). It costs 50 wood to build. It now requires Medieval Storage research.
Tall Cabinet now stores 5 stacks of Food, Drugs and Medicine with a total mass of 30kg. It costs 100 wood to build. It now requires Modern Storage research.
Lockers now stores 10 stacks of apparel with a total mass of 5kg. It costs 60 metalic stuff to build. It now requires Modern Storage research.
Vending Machine now stores up to 10 stacks of small items with a total mass of 20kg and a max mass per item of 0.5kg. It costs 60 metalic stuff to build. It now requires Modern Storage and Cardboard Boxes research.
Steel Barrels now store 4 stacks of chemicals and heavy loose items. It costs 50 steel to build. It requires Modern Storage and Smithing research.
Steel Barrels pallet now stores 36 stacks of chemicals and heavy loose items (9 per tile). It costs 450 steel and 50 wood to build. It requires Modern Storage, Smithing and Pallets research.
Wine Rack now stores 3 stacks of drinkable liquids. It is nice to look at. It costs 50 wood to build. It requires Beer Brewing and Modern Storage research.
Small wooden box now stores 2 stacks of general items with a total mass of 10kg. It costs 20 wood to build. It requires box storage research.
Large wooden box now stores 2 stacks of general items with a total mass of 20kg. It costs 40 wood to build. It requires box storage research.
Pallet with wooden boxes now stores 12 stacks of general items (3 per tile) with a total mass of 160kg (40kg per tile). It costs 330 wood to build. It requires box storage and pallet research.
Small Cardboard box now stores 2 stacks of general items with a total mass of 5kg. It costs 10 wood to build. It requires cardboard research.
Large Cardboard box now stores 2 stacks of general items with a total mass of 10kg. It costs 15 wood to build. It requies cardboard research.
Pallet with Cardboard boxes now stores 12 stacks of general items (3 per tile) with a total mass of 80kg (20kg per tile). It costs 180 wood to build. It requires pallet and cardboard storage research.
Large Pallet now stores 16 stacks of heavy items (4 per tile). It costs 130 wood to build. It now requires Pallet research.
Empty Warehouse Shelf now stores 10 stacks of heavy items (5 per tile). It costs 200 steel to build. It now requires Industrial Storage research.
Warehouse Shelf with Boxes now stores 12 stacks of small items and apparel (6 per tile). It costs 200 steel and 50 wood to build. It requires Industrial Storage and Cardboard research.
Containers now store 40 stacks of small items, apparel or weapons (5 per tile). It costs 650 steel to build. It now requires Industrial Storage research.
Small hay bale now stores 3 stacks of hay. It costs 20 hay to build. It requires Medieval Storage research.
Medium hay bale now stores 5 stacks of hay. It costs 50 hay to build. It requires Medieval Storage research.
Large hay bale now stores 24 stacks of hay (6 per tile). It costs 250 hay to build. It requires Medieval Storage research.
Wooden Wagon now stores 12 stacks of general items (3 per tile). It costs 60 wood to build. It requires Medieval Storage research.
Storage Bags now store 3 stacks of light loose items. It is faster to use with less variety. It costs 30 cloth. It requires Complex Clothing research.
Spacer Container now stores 4 stacks of general items. It costs 80 steel, 30 plasteel, 50 silver and 2 components to build. It requires Modern Storage, Boxes and Fabrication research.
Large Spacer Container now stores 8 stacks of general items (4 per tile). It costs 160 steel, 50 plasteel, 100 silver and 3 components to build. It requires Modern Storage, Boxes and Fabrication research.
Spacer Container Pile now stores 32 stacks of general items (8 per tile). It costs 400 steel, 230 plasteel, 400 silver and 12 components to build. It requires Modern Storage, Boxes and Fabrication research.
Spacer Storage now stores 18 stacks of general items (6 per tile). It costs 200 steel, 150 plasteel, 500 silver and 8 components to build. It requires Modern Storage, Boxes and Fabrication research.
If Vanilla Books Expanded is present, Bookshelf now stores 40 pieces of papers (20 per tile). It costs 50 stuff to build. It now requires Modern Storage research.
If Rimfridge is present, Fridge now stores 4 stacks of food. It now requires Modern Storage research.

Simple Storage Changes

Wooden Basket now stores 3 pieces of apparel with a total weight of 1kg. It now requires Neolithic Storage research.
Barrels now store 3 stacks of drinkable liquids. It is incridibly slow to use if you have variety of liquids in it. It cost 60 Wood. It requires Brewing research.
Barrel Piles now store 10 stacks of drinkable liquids (5 per tile). It costs 200 wood. It requires Brewing research.
Bundles Wrap now store 3 stacks of light loose items. It is faster to use with less variety. It costs 30 cloth. It requires Complex Clothing research.
Bundles Wrap Pile now store 16 stacks of light loose items (4 per tile). It costs 180 cloth. It requires Complex Clothing research.
Bundles Wrap Big now stores 24 stacks of light loose items (6 per tile). It costs 400 cloth. It requires Complex Clothing research.
Metal crate now stores 2 stacks of general items. It still costs 50 steel. It is slow to use. It requires Smithing and Box Storage research.
Small pile of metal crates now store 8 stacks of general items (2 per tile). It costs 200 steel. It is slow to use. It requires Smithing and Box Storage research.
Pile of metal crates now store 12 stacks of general items (3 per tile). It costs 400 steel. It is slower to use. It requires Smithing and Box Storage research.
Big piles of metal crates now store 18 stacks of general items (3 per tile). It costs 600 steel. It is slower to use. It requires Smithing and Box Storage research.
Wooden Crate A now stores 2 stacks of general items (2 per tile) with a total mass of 20kg. It costs 40 wood. It requires Box Storage research.
Wooden Crate A2 now stores 4 stacks of general items (2 per tile) with a total mass of 50kg (25kg per tile). It costs 120 wood. It requires Box Storage research.
Wooden Crate A3 now stores 8 stacks of general items (2 per tile) with a total mass of 100kg (25kg per tile). It costs 200 wood. It requires Box Storage research.
Wooden Crate A4 now stores 12 stacks of general items (3 per tile) with a total mass of 160kg (40kg per tile). It costs 320 wood. It requires Box Storage research.
Wooden Crate B now stores 2 stacks of general items with a total mass of 40kg. It costs 50 wood. It requires Box Storage research.
Wooden Crate c now stores 6 stacks of general items (3 per tile) with a total mass of 80kg (40kg per tile). It costs 150 wood. It requires Box Storage research.
Vending Machines now stores up to 10 stacks of small items with a total mass of 20kg and a max mass per item of 0.5kg. It costs 60 metalic stuff to build. It now requires Modern Storage and Cardboard Boxes research.
Medicine Storage now stores 10 stacks of medical items. It costs 80 metallic stuff and 1 component to build. It now requires Modern Storage research.
Safe now stores 4 stacks of general items. It costs 250 metallic stuff, 50 plasteel and 1 component to build. It now requires Modern Storage and Machining research.
Large Pallet now stores 16 stacks of heavy items (4 per tile). It costs 130 wood to build. It now requires Pallet research.
Large Pallet A now stores 12 stacks of general items (3 per tile) with a total max mass of 90kg (22.5kg per tile). It costs 310 Wood to build. It now requires Pallet and Boxes research.
Large Pallet B now stores 12 stacks of general items (3 per tile) with a total max mass of 90kg (22.5kg per tile). It costs 310 Wood to build. It now requires Beer Brewing, Pallet and Boxes research.
Large Pallet C now stores 12 stacks of general items (3 per tile) with a total max mass of 90kg (22.5kg per tile). It costs 350 Wood to build. It now requires Pallet and Boxes research.
Large Pallet D now stores 8 stacks of general items (2 per tile) with a total max mass of 120kg (30kg per tile). It costs 220 Wood to build. It now requires Pallet and Boxes research.
Large Pallet Can now stores 32 stacks of Chemicals and Heavy Loose Items (8 per tile). It costs 400 metallic stuff and 130 wood to build. It requires Smithing and Pallet research.
Small Pallet now stores 4 stacks of Heavy Items. It costs 40 wood to build. It now requires Pallet research.
Small Pallet Can now stores 4 stacks of Chemicals and Heavy Loose Items. It costs 50 Metallic stuff and 40 wood to build. It requires Smithing and Pallet research.
Small Pallet Crate now stores 2 stacks of general items (2 per tile) with a total mass of 20kg. It costs 40 wood. It requires Pallet and Box Storage research.
Industrial Shelf (empty) footprint is now 5x2. It can store 70 stacks of heavy items (7 per tile) with a total mass of 4500kg (450kg per cell). It costs 750 steel to build. It now requires Industrial Storage and Machining research.
Industrial Shelf (full) footprint is now 5x2. It can store 80 stacks of general items (8 per tile) with a total mass of 4500kg (450kg per cell). It costs 750 steel and 1500 wood to build. It now requires Industrial Storage, Boxes, Pallets and Machining research.
Industrial Dumpsters footprints are now 4x2. They can store 64 stacks of toosable items (6 per tile). They cost 500 steel to build. They require Industrial research.
Silo footprint is now 4x3. It can store 120 stacks of vegetables and plant matter. It costs 600 steel to build. It requires Industrial Storage and Machining research.
Containers footprint is now 5x2. It can store 50 stacks of small items, apparel or weapons (5 per tile). It costs 800 steel to build. It now requires Industrial Storage research.
Small Lockers now stores 10 stacks of apparel with a total mass of 5kg. It costs 60 metalic stuff to build. It now requires Modern Storage research.
Large Lockers now stores 20 stacks of apparel (10 per tile) with a total mass of 10kg (5kg per tile). It costs 60 metalic stuff to build. It now requires Modern Storage research.
Small Military Grade crate now stores 3 stacks of general items with a total mass of 30kg. It costs 100 steel and 30 plasteel to build. It now requires box storage and gunsmithing research.
Pile of Military Grade crates now stores 24 stacks of general items (6 per tile) with a total mass of 200kg (50kg per tile). It costs 400 steel and 120 plasteel to build. It now requires box storage and gunsmithing research.
Long Military Grade crates now stores 12 stacks of general items (3 per tile) with a total mass of 105kg (35kg per tile). It costs 250 steel and 80 plasteel to build. It now requires box storage and gunsmithing research.
Large Military Grade crates now stores 8 stacks of general items (4 per tile) with a total mass of 120kg (60kg per tile). It costs 200 steel and 50 plasteel to build. It now requires box storage and gunsmithing research.
Bank Vault now stores 90 stacks of general items (10 per tile). It costs 500 plasteel, 1000 steel and 5 components to build. It requires Industrial Stores and Machining research.
Chemfuel Storage now stores 10 stacks of chemicals (5 per tile). It costs 150 steel to build. It requires Machining and Industrial Storage research.
Large Chemfuel Storage footprint is now 5x2 and now stores 50 stacks of chemicals (5 per tile). It costs 650 steel and 1 component to build. It requires Machining and Industrial Storage research.
If Vanilla Books Expanded is present, Post Box now stores 20 pieces of papers. It costs 50 stuff to build. It now requires Modern Storage research.
If Yayo's Combat 3 or Combat Extended is present ammo boxes will be present and store ammo only.

Simple Storage: Refrigeration Changes
Refrigerator now stores 8 stacks of food (4 per tile). And costs 200 steel and 4 components to build. It now requires Modern Storage research.
Ice Box now stores 16 stacks of food (4 per tile). And costs 250 steel and 8 components to build. It now requires Modern Storage research.
Refrigerated Box Trucks now stores 40 stacks of food (5 per tile). And costs 800 steel and 15 components to build. It now requires Industrial Storage research.


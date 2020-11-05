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
```
Neolithic               Medieval                Industrial
Neolithic Storage   -> Medieval Storage ->  Modern Storage.
                    -> Storage Boxes    ->  Cardboard Storage
                                            Industrial Storage
                                            Pallets
```

All of the industrial level storage requires Complex Furniture as well.

If, for some reason a research project wouldn't unlock anything, it will be removed.

Most storage buildings will require one (or more) of these research projects. Some will also require specific ones like machining or gun smithing.

### General idea of the new balance.

The rule of thumb for balancing is as follows: The more specific filters the building has, the more stacks it can hold. For example, a Wooden Barrel costs 50 wood and it holds 3 drinkable liquids (like beer), while a Wooden Crate B also costs 50 wood but can only store 2 stacks of general items.

Also, the more stacks (per tile) a building can hold, the more expensive it gets. Lategame storage like Industrial Shelves cost about 750 steel and 1500 wood to build, but can store a massive amount of items.

Lastly, research requeriments are also taken into consideration. Late game storage like Spacer Containers are very powerful, but require Fabrication research.

### Footprint changes

Some items in Simple Storage had problematic footprints. Tall structures would cover the space behind them even if said space was actually empty. This mod modifieds the size of these buildings and offsets the texture to fix this and fit properly ingame. In general this meant that they are smaller ingame.

### ThingDefCategories AKA ingame categories

I decided against adding new categories, as it would make maintance and updating very time consuming. I would have to make patches for almost all mods that add items. The only exception are Fertile Field resources. All of the resources in that mod are loose items (fertilizer, dirt, sand, etc), and so all of them went well together. In order to not clutter the description of loose type storage a lot adding all the individual thingDefs from Fertile Fields, I decided to add this category.

### Removed content

Some buildings in some mod were too problematic to balance around. This problem was mostly due to the small size of some buildings, or the redudancy of their existance. In some other cases, these buildings would have no items that fit in a vanilla game, so they are only added if a fitting mod is found. All the remove content has it's argument for removal in the notes inside the patches.
 
## FAQ

### Where can I see ALL the changes?

This list will probably be outdated at some point, but (here)[https://github.com/Keno-GH/Rebalanced-Deep-Storage/wiki/All-the-changes]

### I found an issue! What can I do?

If you found an issue, please post it (here)[https://github.com/Keno-GH/Rebalanced-Deep-Storage/issues/new]. It would be highly appreciated that you added a complete description of the problem, this way I can work on fixing it quicker. If you fancy, you can follow (this guide)[https://steamcommunity.com/sharedfiles/filedetails/?id=725234314] to get even more info on my way.

### Why can't I store X in this building?

Probably because balancing or visual logic issues, but there is a (very high) chance that I did it wrongly. Please send suggestions through the (issues)[https://github.com/Keno-GH/Rebalanced-Deep-Storage/issues] forum.

## Donations

It would be very highly appreciated! 
<a href='https://ko-fi.com/B0B61GNYP' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi3.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
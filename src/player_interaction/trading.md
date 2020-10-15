# Trading

This section will introduce you to the `$trade` command, as well as other ways to trade certain types of items.

## Crates

To see what crates you have, `$crates` gives a breakdown by each type. Crates can be opened (`$open [type]`), sold, traded or given to other IdleRPG players.

Crate drop chances for range of stats from each crate rarity:

_we gotta find a way to add emojis here_

- Common:
  - 50 %: 1-9
  - 30 %: 10-19
  - 20 %: 20-30
- Uncommon:
  - 50 %: 10-19
  - 30 %: 20-29
  - 20 %: 30-35
- Rare:
  - 50 %: 20-29
  - 30 %: 30-34
  - 20 %: 35-40
- Magic:
  - 50 %: 30-34
  - 30 %: 35-40
  - 20 %: 41-45
- Legendary:
  - equally likely: 41-50

_is there a way to make this into a comprehensive table?_  
_also, we need text on how to actually get crates_

## Items

Items are equippable weapons that you can use to increase your adventure survivability rate, and make you stronger in all battle-related aspects of the game.

You can get items by finishing adventures, buying them off the market or other players, opening crates or buying them off `$trader`.  
There are two main categories of items, two handed and single handed, while single handed weapons can be further categorised into left handed, right handed, or any handed.  
All items deal damage except for the shield, as the shield gives you armor.

### Types

| Item Type | Hand  | Description                                                                                                                                                                             |
| --------- | ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Axe       | any   | An any handed weapon that has an axe head attached to a handle.                                                                                                                         |
| Dagger    | any   | An any handed weapon that is a short knife with a pointed and a double edged blade.                                                                                                     |
| Hammer    | any   | An any handed weapon with a heavy metal head mounted at right angles at the end of a handle.                                                                                            |
| Knife     | any   | An any handed weapon that is sharp but single edged.                                                                                                                                    |
| Sword     | any   | An any handed weapon with a long metal blade and a hilt with a hand guard. It is one of the older item types in the game.                                                               |
| Shield    | left  | A left handed item that protects you from damage, it is the only item in the game that gives you armor. It is also one of the older item types in the game that came along with swords. |
| Spear     | right | A right handed weapon with a pointed tip, typically of steel, and a long shaft, used for thrusting or throwing.                                                                         |
| Wand      | right | A right handed weapon that is a stick with a rune attached at the end.                                                                                                                  |
| Bow       | both  | A two-handed weapon that is a curved piece of material that forms a C-shape with a string on the two tips, arrows are automatically in bows and are infinite.                           |
| Howlet    | both  | A long black stick used as a two-handed blunt weapon.                                                                                                                                   |
| Scythe    | both  | A two handed weapon used for cutting crops such as grass or wheat, with a long curved blade at the end of a long pole attached to which are one or two short handles.                   |

> **Note**: Both handed weapons (also known as 2-handed weapons) can only be equipped one at a time, right handed means it's a single handed weapon that you can only use on your right hand; similarly for left, and any means it's a single handed weapon that can be equipped on either hand.  
> You cannot have two right handed weapons equipped at the same time, nor too left handeds. You can, however, have two any-handed weapons at a time. The equip logic in IdleRPG will let you know if there was an error while equipping.

### Stat

The stat of an item determines how effective it is, the higher an item's stat is, the more effective it is.

Stats means both armor and damage. If a shield has a 41 stat, it means the shield will give you 41 armor and 0 damage. If an any damage dealing weapon's stat is 41, it means it will do 41 damage and 0 armor.  
Some other ways you can obtain stats are by races, which give you a total of 4 stats, as well as classes such as warrior, which gives 1 extra armor stat per evolution.

The highest stat a single handed item can be is 50, which _can_ be obtained by opening a legendary crate. The highest stat a two-handed weapon can be is 100, which, too, can be obtained by opening a legendary crate.

### Upgrading

Upgrading is a feature which allows you to increase an item's stat.

The stat of an item can be upgraded up to stat 41 for single handed weapons and 82 for two-handed weapons.  
The only way to get an item greater than 41 for single handed items and 82 for two-handed weapons is by opening high rarity crates or buying them from other players.

To upgrade an item's stat, use `$upgrade [ItemID]`. This will prompt a confirmation message which you can agree to by reacting with ✅.  
Upgrading an item's stat costs 250 times the stat you are upgrading, which means, for an example, upgrading an 80 stat item costs \$20,000, as 250×80 is 20,000.

## Money

_section unfinished_

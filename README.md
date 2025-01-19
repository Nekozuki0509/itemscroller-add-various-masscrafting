![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/Nekozuki0509/itemscroller-add-various-masscrafting/total?logo=github&color=blue)
[![Discord](https://img.shields.io/discord/1241236305741090836?logo=discord&color=5765f2)](https://discord.gg/352Cdy8MjV)
[![Static Badge](https://img.shields.io/badge/litlink-Nekozuki0509-9594f9)](https://lit.link/nekozuki0509)
## itemscroller-various-masscrafting is not Masa's original itemscroller. If you have issues with this mod, please contact Nekozuki0509 (or open a bug report here).
## Note
This is a customized version of Andrews54757's itemscroller-crafting-fix mod that add various masscrafing for 1.20.1. Andrews54757's original mod can be found [here](https://github.com/Andrews54757/itemscroller-crafting-fix)



itemscroller-crafting-fix
==========================

## Note
This is a customized version of Masa's itemscroller mod that fixes crafting features for 1.18. Masa's original mod can be found [here](https://github.com/maruohon/itemscroller)

Customizations:
* More accurate/faster crafting through recipe book protocol
* Toggleable crafting (so you can keep crafting without holding down a key, eg for crafting millions of pistons)
* Honey crafting

- Removed carpetControlQ crafting option as it causes a "slow crafting issue"
- Removed packetRateLimit as it may lead to problems.

### What's different?
Post 1.13, Mojang has changed the crafting mechanics of the game. Before 1.13, crafting was very fast as much of the logic was handled client-side. In 1.13, most of the crafting logic was moved to the server. This broke Itemscroller's fast crafting features, since every ingredient now had to be moved one slot at a time to the crafting grid for it to work. This drastically worsened server-client desync, a compounding problem, leading to an increasing number of failed crafting attempts and accidental ingredient leaks which made afk crafting impossible. 

This customized version of the mod, fixes the problem by handling ingredient movement server-side using the recipe book protocols when it can. 

**Note: Some recipes like fireworks rockets that are not in the recipe book do not take advantage of this protocol, in those cases old itemscroller methods will be used**

Item Scroller
==============
Item Scroller is a Minecraft mod that adds various convenience features for moving items
inside inventory GUIs. Examples are scrolling the mouse wheel over slots with items in them
or Shift/Ctrl + click + dragging over slots to move items from them in various ways etc.

Item scrolling is basically what the old NEI mod did and Mouse Tweaks also does.
This mod has some different drag features compared to Mouse Tweaks, and also some special
villager trading related helper features as well as crafting helper features.

For more information and downloads of the already compiled builds,
see https://www.curseforge.com/minecraft/mc-mods/item-scroller

Compiling
=========
* Clone the repository
* Open a command prompt/terminal to the repository directory
* run 'gradlew build'
* The built jar file will be in build/libs/

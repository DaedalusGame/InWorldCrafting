# 1.12.2

## 1.2.0
- Removed redundant method overloading for Fluid crafting. All inputitems should now always be wrapped with array brackets. This will BREAK previous scripts that do not surround ingredients with the array brackets.

## 1.1.2
- Fixed Crash when batch Crafting.

## 1.1.1
- Fixed FluidToItem JEI category, outputs where not aligned correctly.

## 1.1
- FluidToFluid and FluidToItem recipes now take multiple inputs. (Thanks ExpensiveKoala)
- Altered FluidToFluid and FluidToItem JEI categories to fit more inputs.
- Added particles to give visual feedback to the player upon completed crafts.

## 1.0
- Removed the item blacklist, changed approach to crafting so we don't cannibalized custom EntityItem classes. (Might be a bit more expensive on the cpu, so marking this version as a beta)
- Fixed a bug where Fluid to Item recipes that consumes the fluid could craft in flowing fluid.
- Inputs that are not consumed during crafting will now properly update it's shrunken state.
- Removed config as the Blacklist is no longer a thing, the config file can be removed without breaking anything.

## 0.13
- Added NBT matching for ingredients

## 0.12
- Fixed a crash for OpenJDK users.

## 0.11
- Added Input blacklist for items from other mods that require their own EntityItem logic.
- Added config option to disable said blacklist.

## 0.10
- Merged custom entities so that one specific input can do multiple types of crafting instead of picking the first matching recipe.
- Added Fire Crafting.
- Added Explosion Crafting.
- Refactored project to reflect the new Name.
- Will break current scripts. Change imports to mods.inworldcrafting instead of mods.fluidtransformtweaker
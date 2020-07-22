# Construction

## Table of Contents

- **Construction** (Current Page)
- [Gameplay](Gameplay.md)
- [Misc.](Misc.md)
- [Dropped Features](Dropped.md)

## Terminology

- Block - The smallest unit of space a buildable object can fill. Uniform in dimensions.
- Cell - The unit of space claimed by placing a totem. Cells are fairly large, containing possibly 50x50x50 blocks.

## Building Mechanics

- The construction system allows for players to construct buildings and place machines with useful functionality almost anywhere in the world.
- The construction system mimics other construction systems in the genre (Rust, Hurtworld) but with significant differences.
- The construction system is constrained to a Minecraft-like 3D grid.

## Building Parts

|                | Area (WxDxH) |
| -------------- | ------------ |
| Foundation     | 4x4x6        |
| Ramp           | 2x3x2        |
| Doorway + Door | 2x1x3        |
| Pillar         | 1x1x3        |
| Wall           | 4x1x4        |
| Staircase      | 4x4x4        |
| Ceiling        | 4x4x1        |
| Window         | 1x1x1        |

## Machines & Doodads

- Totem/Stake/Claim- Claims a cell and grants building privileges and door access to anyone authorized. Only 1 totem is allowed per cell. Anyone can authorize/deauthorize by interacting with the totem. A player's authorization cannot be cleared by any other player, only himself. Totems cannot be removed with a building hammer, only destroyed with weapons. Totems have around 1500hp.
- Sleeping Bag - Cheap. Respawn once every 5 mins. Each player is allowed 1 per cell.
- Bed - Expensive. Respawn once every 5 mins. No limit.
- Workbench - Allows you to craft faster while standing within 4m.
- Camp Fire - Used for cooking food and smelting ore. Heals nearby players very slowly over time. Disappears when fuel depletes.
- Barbecue - Used for cooking food and smelting ore. Heals nearby players very slowly over time.
- Blast Furnace - Used for disassembling tools and weapons into raw material.
- Small Storage - 25 slots
- Large Storage - 50 slots. 2x cost of small storage
- Barricade - Deployable wall for defense. 3 blocks wide by 2 blocks high. Is destructible by weapons and has ~600hp. Can be placed anywhere regardless of totem ownership. Cannot be placed on unclimbable slopes. This is the only object in the game not restricted to the construction grid which means it can be placed at any angle.

# Construction #
The construction system allows for players to construct buildings and place machines with useful functionality almost anywhere in the world. This construction system mimics other constuction systems in the genre (Rust, Hurtworld) but with significant differences.

The construction system is constrained to a Minecraft-like, 3D, grid. Each piece in this grid will be referred to as a ***block*** hereafter. Each *block* is uniform in dimension.

Building pieces and doodads cannot cover less than a single block. Building pieces *can* cover more than a single block (foundations and walls, for example).


### Building Parts ###
|                   | Area (WxDxH)  |
| ----------------- | ------------- |
| Foundation        | 4x4x6         |
| Ramp              | 2x3x2         |
| Doorway + Door    | 2x1x3         |
| Pillar            | 1x1x3         |
| Wall              | 4x1x4         |
| Staircase         | 4x4x4         |
| Ceiling           | 4x4x1         |
| Window            | 1x1x1         |


### Machines & Doodads ###
|                   | Description   |
| ----------------- | ------------- |
| Sleeping Bag      | Cheap. Respawn once every 5 mins. Each player is allowed 1 per cell. |
| Bed               | Expensive. Respawn once every 5 mins. No limit. |
| Workbench         | Allows you to craft faster while standing within 4m |
| Camp Fire         | Used for cooking food and smelting ore. Heals nearby players very slowly over time. Disappears when fuel depletes. |
| Barbecue          | Used for cooking food and smelting ore. Heals nearby players very slowly over time. |
| Blast Furnace     | Used for disassembling tools and weapons into raw material. |
| Totem             | Claims a cell and grants building privileges and door access to anyone authorized. Only 1 totem is allowed per cell. Anyone can authorize/deauthorize by interacting with the totem. A player's authorization cannot be cleared by any other player, only himself. Totems cannot be removed with a building hammer, only destroyed with weapons. Totems have around 1500hp. |
| Small Storage     | 20 slots |
| Large Storage     | 50 slots |
| Barricade         | A small fence; 3m wide x 2m high. Is destructible by weapons and has ~600hp. Can be placed anywhere regardless of totem ownership. Cannot be placed on unclimbable slopes. |
| Transfer box      | A 1-slot container you can place on a wall; lootable from both sides of the wall. Doesn't require ownership to place. Useful for transfering items out of a base you're stuck inside. | 


### Misc. ###
All interactable objects in the world interact immediately; on `OnKeyPressed`. The exception to this is doors, which will open when `OnKeyPressed` and `OnKeyReleased` are called within 500ms of eachother. Past 500ms, if the player is still holding 'interact' on a door, the door is considered ***held***. The mechanics of a held door is as follows:
 - A held door is uninteractable by other players until the player holding the door releases his 'interact' key.
 - While holding a door, the player's camera is locked.
 - Doors can be held regardless of ownership privileges.
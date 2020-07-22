# Dropped Features

## Table of Contents

- [Construction](Construction.md)
- [Gameplay](Gameplay.md)
- [Misc.](Misc.md)
- **Dropped Features** (Current Page)

## Transfer Box (Machines & Doodads)

A 1-slot container you can place on a wall; accessible from both sides of the wall. Doesn't require ownership to place. Useful for transferring items out of a base you're stuck inside.

> 7/21/2020: Dropped because it gives groups an advantage over solo players.

## Door Holding (Building Mechanic)

All interactable objects in the world interact immediately on `OnKeyPressed`. The exception to this is doors, which open when `OnKeyPressed` and `OnKeyReleased` are called within 500ms of each other. Past 500ms, if the player is still holding 'interact' on a door, the door is considered **_held_**. The mechanics of a held door is as follows:

- A held door is not interactable by other players until the player holding the door releases his 'interact' key.
- While holding a door, the player's camera is locked.
- Doors can be held regardless of ownership privileges.

> 7/21/2020: Dropped because it gives groups an advantage over solo players.

## Disposable Ammo (Gameplay Mechanic)

- All gun ammunition exists in magazine form. There are no individual bullets.
- Magazines _always_ contain max capacity.
- Magazines can be crafted or found in loot boxes.
- Reloading a gun consumes an entire magazine from your inventory.
- Reloading a gun overwrites any unspent ammo in the gun. If you have 5 bullets left before reloading, those 5 bullets are deleted.
- Magazines each take up 1 inventory slot.

> 9/14/16: Adds extra complexity/skill to fights. Instead of reloading being a mindless action (always spam R behind corners) you'll need to decide if wasting ammo is worth having extra ammo available in the next fight.
>
> 4/23/18: I'm afraid this mechanic might give highly geared players an even greater advantage than they would otherwise have over lower geared players. Of course a highly geared player will be holding many more magazines than a low-tier player and thus can use this ammo mechanic to his advantage, but then the low-tier player has potentially more to gain by killing a player who's carrying a lot of extra ammo.

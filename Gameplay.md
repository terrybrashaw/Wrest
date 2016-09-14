# Gameplay #

### Movement ###
Basic movement:
 - Running (100% movement speed)
 - Walking (*Forward* @ 49%, *Sidestrafing* @ 49%, *Backwards* @ 34%)
 - Crouching (29%)
 - Jumping

Advanced movement:
- **Bunny Hopping** - While mid-air, landing on a down-angled slope and jumping again within ~50ms of landing will increase velocity.

Movement facts:
- You can only run forward.
- Moving while crouching is completely silent; produces no footstep noise. 
- Crouching while mid-air pulls your legs up while your upper-body and head are kept in the same position. This detail is important because:
    - It allows you to *crouch-jump* onto high places.
    - Your head movement should stay predictable to enemies, even when you're jumping and crouch-spamming.
- Slopes angled at >75 degrees are unclimbable.
- You can safely fall a distance of <4 body lengths with no penalty.
- You cannot stand on another player or use them in any way to boost onto higher areas.
- Falling >4 body lengths will break your leg, causing 55% damage and applying a `slowed` debuff for 25 seconds. The amount of damage dealt does not vary between 4-12 body lengths.
- Falling >12 body lengths kills you instantly.


### Gunplay ###
- Recoil does not reset automatically.
- 2 modes of shooting, hipfire and ADS (aiming-down-sights).
- Hipfire is pinpoint accurate; massive recoil.
- ADS is pinpoint accurate; reduced recoil.
- Crosshairs will show for hipfiring.


### Ammo Mechanics ###
- All gun ammunition exists in magazine form. There are no individual bullets.
- Magazines *always* contain max capacity.
- Magazines can be crafted or found in loot boxes.
- Reloading a gun consumes an entire magazine from your inventory.
- Reloading a gun overwrites any leftover ammo. If you have 5 bullets left before reloading, those 5 bullets are deleted.
- (*Maybe*) Instead of deleting leftover ammo, it's converted to equivalent raw materials.
- Magazines each take up 1 inventory slot.
- All magazines contain tracers every third shot; as well as three consecutive tracers at the bottom.

Why?
- Adds extra complexity/skill to fights. Instead of reloading being a mindless action (always spam R behind corners) you'll need to decide if wasting ammo is worth having extra ammo available in the next fight.
- Ultimately, this is a nerf to guns in some way. This makes melee weapons and bows stronger.


### Equipment ###
Armor slots:
 - Head
 - Body
 - Legs
 - Feet

Armor tiers:

|          | Head  | Body  | Legs  | Feet  |
| -------- | ----- | ----- | ----- | ----- |
| Cloth    | 10-10 | 10-10 | 5-5   | 8-8   |
| Leather  | 10-15 | 10-15 | 10-10 | 10-10 |
| Kevlar   | 25-25 | 30-30 | 15-15 | 15-15 |

Tools and weapons:

|            | Damage | Range | Cooldown | Reload Time | Ammo | Recoil | Mode      | Projectile Speed |
| ---------- | ------ | ----- | -------- | ----------- | ---- | ------ | --------- | ---------------- |
| Hammer     | -      | -     | -        | -           | -    | -      | -         | -                |
| Hatchet    | 25     | 2m    | 1s       | -           | -    | -      | -         | -                |
| Pickaxe    | 45     | 2m    | 3s       | -           | -    | -      | -         | -                |
| Bow        | 34     | 250m  | 0.4s     | -           | -    | -      | -         | 60m/s            |
| Pistol     | 34     | 120m  | 0.1s     | 2s          | 8    | 11     | Single    | Hitscan          |
| Shotgun    | 180    | 30m   | 1.45s    | 4s          | 6    | 15     | Single    | Hitscan          |
| Auto Rifle | 35     | 130m  | 0.125s   | 3s          | 30   | 8      | Automatic | Hitscan          |
| Bolt Rifle | 63     | 250m  | 2.2s     | 5s          | 3    | 14     | Single    | Hitscan          |

The shotgun's spray pattern will be similar to Reflex.

Weapon attachments:
 - Red Dot Sight
 - Silencer

Grenades:
 - Flashbang
 - Smoke
 - HE Grenade
 - Molotov

Grenade physics will be identical to CS:GO.

### Hotbar and Inventory ###
6 slots for your hotbar.  
24 slots for your inventory.  
30 slots total.

Moving items in your inventory:
 - Move an item by dragging and dropping onto an empty slot.
 - Swap an item by dragging and dropping onto another item.
 - Drop an item by dragging and dropping outside of the inventory window.

Helpful item movement mechanics:
 - Split a stack of items in half by holding `Shift` before dragging and dropping.
 - Pick up 1 from a stack of items by holding `Ctrl` before dragging and dropping.
 - Pick up all-but-1 from a stack of items by holding `Alt` before dragging and dropping.
 - To "drag and drop" items, they can either be:
  - Click and hold while moving, release to drop.
  - Click to pick up, click to drop.

Quick-using items in your inventory: 
 - Use an item by right clicking it. Only some items will have a quick-action, for example: food will have an "Eat" action and guns will have an "Unload" action.
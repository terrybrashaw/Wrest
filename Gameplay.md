# Gameplay #

## Movement ##
Basic movement:
* Running (100% movement speed)
* Walking (Forward @ 50%, Sidestrafing @ 50%, Backwards @ 35%)
* Crouching (30%)
* Jumping

Advanced movement:
* Circle Jumping - Works similar to Reflex's Circle Jump.

Movement mechanics:
* You can only run forward; you cannot run while sidestrafing.
* There is air-control.
* Moving while crouching is completely silent; produces no footstep noise. 
* Crouching while mid-air pulls your legs up while your upper-body and head are kept in the same position. This detail is important because:
    * It allows you to *crouch-jump* onto high places.
    * Your head movement should stay predictable to enemies, even when you're jumping and crouch-spamming.
* Slopes angled at >75 degrees are unclimbable, you simply slide down.
* You cannot stand on another player or use them in any way to boost onto higher areas.
* You can safely fall a distance of <4 body lengths with no penalty.
* Falling >4 body lengths will break your leg, causing 55% damage and applying a `slowed` debuff for 25 seconds. The amount of damage dealt does not vary between 4-12 body lengths.
* Falling >12 body lengths kills you instantly.


## Gunplay ##
* Recoil does not reset automatically.
* You can shoot in any state of movement besides running.
* 2 modes of shooting: hipfire and ADS (aiming-down-sights).
* Hipfire:
    * 100% accurate
    * Massive recoil
    * On-screen crosshair
* ADS:
    * 100% accurate
    * Normal recoil
    * Slight amount of zoom
    * Slight amount of sway


## Ammo Mechanics ##
* All gun ammunition exists in magazine form. There are no individual bullets.
* Magazines *always* contain max capacity.
* Magazines can be crafted or found in loot boxes.
* Reloading a gun consumes an entire magazine from your inventory.
* Reloading a gun overwrites any leftover ammo. If you have 5 bullets left before reloading, those 5 bullets are deleted.
* Magazines each take up 1 inventory slot.

Personal theory on this ammo mechanic:
* Adds extra complexity/skill to fights. Instead of reloading being a mindless action (always spam R behind corners) you'll need to decide if wasting ammo is worth having extra ammo available in the next fight.


## Equipment ##
Armor slots:
* Head
* Body
* Legs
* Feet

Armor tiers:

|          | Head  | Body  | Legs  | Feet  |
| -------- | ----- | ----- | ----- | ----- |
| Cloth    | 10-10 | 10-10 | 5-5   | 8-8   |
| Leather  | 10-15 | 10-15 | 10-10 | 10-10 |
| Kevlar   | 25-25 | 30-30 | 15-15 | 15-15 |

Tools and weapons:

|            | Damage | Range | Ammo | Cooldown | Reload Time | Recoil | Mode      | Projectile Speed |
| ---------- | ------ | ----- | ---- | -------- | ----------- | ------ | --------- | ---------------- |
| Hatchet    | 25     | 2m    | -    | 1s       | -           | -      | -         | -                |
| Pickaxe    | 45     | 2m    | -    | 3s       | -           | -      | -         | -                |
| Bow        | 34     | 250m  | -    | 0.4s     | -           | -      | -         | 60m/s            |
| Pistol     | 34     | 120m  | 8    | 0.1s     | 2s          | 11     | Single    | Hitscan          |
| Shotgun    | 180    | 30m   | 6    | 1.45s    | 4s          | 15     | Single    | Hitscan          |
| Auto Rifle | 35     | 130m  | 30   | 0.125s   | 3s          | 8      | Automatic | Hitscan          |
| Bolt Rifle | 63     | 250m  | 3    | 2.2s     | 5s          | 14     | Single    | Hitscan          |

Notes:
* The shotgun's spray pattern is static, similar to Reflex.


### Hotbar and Inventory ###
* 6 slots for your hotbar.  
* 24 slots for your inventory.  
* 30 slots total.

Moving items in your inventory:
* Move an item by dragging and dropping onto an empty slot.
* Swap an item by dragging and dropping onto another item.
* Drop an item by dragging and dropping outside of the inventory window.

Helpful item movement mechanics:
* Split a stack of items in half by holding `Shift` before dragging and dropping.
* Pick up 1 from a stack of items by holding `Ctrl` before dragging and dropping.
* Pick up all-but-1 from a stack of items by holding `Alt` before dragging and dropping.
* To "drag and drop" items, they can either be:
    * Click and hold while moving, release to drop.
    * Click to pick up, click to drop.

Quick-using items in your inventory:
* Use an item by right clicking it. Only some items have a quick-action, for example: food has an "Eat" action.


### Events ###
Airdrops:
* A plane flies over the map, dropping loot crates
* Airdrops drop BETWEEN 1-3 crates along the plane's travel path.
* Airdrop crates ALWAYS contain items.
* Airdrop crates ALWAYS contain some significantly valuable items.
* Airdrop crates ALWAYS contain a randomized assortment of items.
* Selected airdrop locations follow a pattern. Example:
    * For towns A, B, C, D, each subsequent airdrop will be dropped at the next location
    * A, B, C, D, A, B, C, D, A, B, C, D...
* Airdrop frequency follows a curve:
    * Infrequent drops between 0%-35% server capacity
    * Frequent drops between 35%-80% server capacity
    * Infrequent drops between 80%-100% server capacity
    * Infrequent = every 2 hours
    * Frequent = every hour

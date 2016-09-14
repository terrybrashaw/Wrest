### Movement ###
###### Basic Movement ######
 - Walking (`Forward` at 3.8m/s, `Sidestrafing` at 3.8m/s, `Backward` at 2.7m/s)
 - Running (7.9m/s)
 - Crouching (2.3m/s)
 - Jumping

Moving while crouching is completely silent; produces no footstep noise. 

Crouching while mid-air pulls your legs up while your upper-body and head are kept in the same position. This detail is important because:

 - It allows you to *crouch-jump* onto high places.
 - Your head movement should stay predictable to enemies, even when you're jumping and crouch-spamming.

Slopes angled at >75 degrees are unclimbable.

You can safely fall at a distance of <4 body lengths with no penalty.

You cannot stand on another player or use them in any way to boost onto higher areas.

Falling >4 body lengths will break your leg, causing 55% damage and applying a `slowed` debuff for 25 seconds. The amount of damage dealt does not vary between 4-12 body lengths.

Falling >12 body lengths kills you instantly.


###### Advanced Movement ######
 - **Bunny Hopping** - While mid-air, landing on a down-angled slope and jumping again within ~50ms of landing will increase velocity.


### Equipment ###
###### Armor Slots ######
 - Head
 - Body
 - Legs
 - Feet

###### Armor ######
|          | Head  | Body  | Legs  | Feet  |
| -------- | ----- | ----- | ----- | ----- |
| Cloth    | 10-10 | 10-10 | 5-5   | 8-8   |
| Leather  | 10-15 | 10-15 | 10-10 | 10-10 |
| Kevlar   | 25-25 | 30-30 | 15-15 | 15-15 |

###### Tools & Weapons ######
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

The shotgun's spray will have a set pattern similar to Reflex or Quake.

###### Weapon Attachments ######
 - Red Dot Sight
 - Silencer

###### Grenades ######
 - Flashbang
 - Smoke
 - HE Grenade
 - Molotov

Grenade physics will be identical to CS:GO.


### Gunplay ###
- Recoil does not reset automatically.
- 2 modes of shooting, hipfire and ADS (aiming-down-sights).
- Hipfire is pinpoint accurate; massive recoil.
- ADS is pinpoint accurate; reduced recoil.
- Crosshairs will show for hipfiring.


### Ammo Mechanics ###
- All gun ammunitian exists in magazine form. There are no individual bullets.
- Magazines *always* contain max capacity.
- Magaines can be crafted or found in loot boxes.
- Reloading a gun consumes an entire magazine from your inventory.
- Reloading a gun overwrites any leftover ammo. If you have 5 bullets left before reloading, those 5 bullets are deleted.
- (*Maybe*) Instead of deleting leftover ammo, it's converted to equivalent raw materials.
- Magazines each take up 1 inventory slot.
- All magazines contain tracers every third shot; as well as three consecutive tracers at the bottom.

Why?
- Adds extra complexity/skill to fights. Instead of reloading being a mindless action (always spam R behind corners) you'll need to decide if wasting ammo is worth having extra ammo available in the next fight.
- Ultimately, this is a nerf to guns in some way. This makes melee weapons and bows stronger.

### Environment ###
###### Day/Night Cycles ######
Day:Night ratio will be around 7:3

Nighttime atmosphere will be equivalent to *Death Valley* in BF:3. Perfectly visible, blue post-process tint, brightened lights/fires.


### User Interface ###
###### Hotbar & Inventory ######
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


###### In-game Overlays ######
Player names are only visible when standing close to a player and holding your crosshair over them. Similar to CS:GO.



### Experimental Miscellaneous Ideas ###
 - A tool should be built to find any terrain geometry angled near the 'gray area' of the walkable/unwalkable range (65-75 degrees). This geometry should be rounded (making it slightly steeper or flatter) to make terrain more readable.

 - Players can be knocked out (or *downed*) instead of killed in some situations. I haven't what these situations are but it shouldn't interfere with impressive kills. For example: getting a killing blow with a headshot should always kill.

 - I'd like to explore the concept of food items being the main method of healing. There would be a different food type that drops from each mob that can be eaten raw, cooked, or combined with other items to create more exotic food. Each food item would have it's own advantage.

 - Shallow lakes, about a foot deep. Used for fishing; players can set fish traps to 'farm' fish. Players can drink from them to restore health.

 - When a player is killed, instead of turning their player model into a ragdoll, they could be broken up into vertices and disintegrate. The vertices at the location of the killing blow would expand and travel in the same trajectory as the projectile that caused the killing blow. So a fatal headshot would cause the head to 'explode' while the rest of the body disintegrates in-place almost.

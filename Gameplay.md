# Gameplay

## Table of Contents

- [Construction](Construction.md)
- **Gameplay** (Current Page)
- [Misc.](Misc.md)
- [Dropped Features](Dropped.md)

## Movement

Basic movement:

- Running (100% movement speed)
- Walking (Forward @ 50%, Sidestrafing @ 50%, Backwards @ 35%)
- Crouching (30%)
- Jumping

Advanced movement:

- Circle Jumping - Works similar to Reflex's Circle Jump.

Movement mechanics:

- You can only run forward; you cannot run while sidestrafing.
- There is air-control.
- Moving while crouching is completely silent; produces no footstep noise.
- Crouching while mid-air pulls your legs up while your upper-body and head are kept in the same position. This detail is important because:
  - It allows you to _crouch-jump_ onto high places.
  - Your head movement should stay predictable to enemies, even when you're jumping and crouch-spamming.
- Slopes angled at >75 degrees are unclimbable, you simply slide down.
- You cannot stand on another player or use them in any way to boost onto higher areas.
- You can safely fall a distance of <4 body lengths with no penalty.
- Falling >4 body lengths will break your leg, causing 55% damage and applying a slow effect for 25 seconds. The amount of damage dealt does not vary between 4-12 body lengths.
- Falling >12 body lengths kills you instantly.

## Gunplay

- Recoil does not reset automatically.
- You can shoot in any state of movement besides running.
- 2 modes of shooting: hipfire and aiming-down-sights.
- Hipfire:
  - 100% accurate
  - Massive recoil
  - On-screen crosshair
- ADS:
  - 100% accurate
  - Normal recoil

## Equipment

Armor slots:

- Head (2 tiers; Hat < Mask)
- Torso (2 tiers; T-Shirt < Long Sleeve)
- Legs (2 tiers; Shorts < Pants)
- Hands (1 tier)
- Feet (1 tier)

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

- The shotgun's spray pattern is static, similar to Reflex.

Possible weapons that have interesting mechanics but no concrete stats:

- Spear - Toggle between _melee_ and _throw_ modes. Similar to Hurtworld's spear.
- SMG - Auto rifle with low recoil and low damage.

## Hotbar and Inventory

- 24 slots for your inventory.
- 6 slots for your hotbar.
- 30 slots total.

The mechanics of inventory management prioritize a high skill ceiling. Items must be manually moved from slot to slot; there is no automated looting/unlooting.

- Move an item by dragging and dropping onto an empty slot.
- Swap an item by dragging and dropping onto another item.
- Drop an item by dragging and dropping outside of the inventory window.
- Split a stack of items in half by holding <kbd>Shift</kbd> while dragging and dropping.
- Pick up 1 item from a stack of items by holding <kbd>Ctrl</kbd> while dragging and dropping.
- Pick up all-but-1 item from a stack of items by holding <kbd>Alt</kbd> while dragging and dropping.
- Use an item by right clicking it (if applicable). For example: food can be right-clicked to eat.

## Events

### Airdrops

- A plane flies over the map, dropping loot crates
- Airdrops drop BETWEEN 1-3 crates along the plane's travel path.
- Airdrop crates ALWAYS contain items.
- Airdrop crates ALWAYS contain some significantly valuable items.
- Airdrop crates ALWAYS contain a randomized assortment of items.
- The location selected for the next airdrop follows a repeating pattern. If there are 4 airdrop locations — A, B, C, D — the locations would be chosen repeating order: A, B, C, D, A, B, C, D, A, B, C, D...
- The repeating pattern of airdrops locations is server-dependent; each server has its own unique pattern.
- Airdrop frequency follows a curve:
  - Infrequent drops between 0%-35% server capacity
  - Frequent drops between 35%-80% server capacity
  - Infrequent drops between 80%-100% server capacity
  - Infrequent = every 2 hours
  - Frequent = every hour

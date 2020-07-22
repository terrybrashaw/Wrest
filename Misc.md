# Misc

## Table of Contents

- [Construction](Construction.md)
- [Gameplay](Gameplay.md)
- **Misc** (Current Page)

## Environment

- Day:Night ratio is around 3:1
- Nighttime atmosphere is equivalent to _Death Valley_ in BF:3. Perfectly visible, blue post-process tint, brightened lights/fires.

## Sound Design

Guns
5 main sound components involved in gun sounds:

1. Gunshot
2. Initial wave
3. Echo
4. Bullet crack
5. Bullet whiz

- When close to the gunshot source: **Gunshot** followed by a delayed **echo**
- When far from the source AND near the bullet trajectory AND within weapon hit range: **Bullet crack** followed almost immediately by the **initial wave** followed by an **echo**
- When far from the source AND near the bullet trajectory BUT outside weapon hit range: **Bullet whiz** followed by a slightly delayed **initial wave** followed by an **echo**
- When far from the source AND far from the bullet trajectory: **Initial wave** followed by an **echo**

With these rules, you can gain some information based on the sounds:

1. Most obviously, when being directly shot at, you can tell immediately if you are in range of the player shooting.
2. Based on the delay between the **initial wave** and the **echo**, you can obtain a rough idea of the distance from you to the shooter. A short delay means you are far; a long delay means you are near.

## User interface

- Player names are only visible when standing close to a player and holding your crosshair over them. Similar to CS:GO.

## Experimental ideas

- A tool should be built to find any terrain geometry angled near the 'gray area' of the walkable/unwalkable range (65-75 degrees). This geometry should be rounded (making it slightly steeper or flatter) to make terrain more readable.

- I'd like to explore the concept of food items being the main method of healing. There would be a different food type that drops from each mob that can be eaten raw, cooked, or combined with other items to create more exotic food. Each food item would have it's own advantage.

- Shallow lakes, about a foot deep. Used for fishing; players can set fish traps to 'farm' fish.

- In towns, there should be interactable objects that, when activated, draw attention of players from a large distance. For example: a bell in a tower you can ring.

- When shooting guns, play an additional sound to signal low ammo when ammo is below 7 shots or something.

- Rust has a pretty good mechanic where farming can be optimized by hitting randomly appearing "X" marks on rocks or trees.

- I've settled on 3 main rad towns connected by a _main_ road. There will of course be other wreckages and ruins and maybe even small undamaged outposts.

- Have two communication towers in each rad town for communicating with the other rad tows. Each tower has "straight key" morse code machines to send signals, and speakers to receive signals. I think this would be a small win for encouraging interaction between players over long distances. If someone is sending signals from a different rad town, you know where to look for people to fight. (Small note: to emphasize where the towers are leading to, have utility poles connect them along the main road)

## End-game possibilities

Battle Royale:

- Before a server-wipe the server goes into a Battle Royale.
- Harmful gas closes in on a randomly selected bunker over a period of 15-20 minutes
- Last player alive wins.

## Things to keep in mind

- Keep walls flat <https://youtu.be/kapUHDkeCE8>
- ESP Honeypot
- Trains (WoW-style transportation with big platforms that move on a rail)
- Each type of mob should have its own distinct mechanic, similar to Doom or Serious Sam
- Anything interactable should have an emmisive green glow pattern somewhere. (Doors, chests, beds, machines)

## Server settings

- The server decides which languages are allowed.

## Removed

- **Bunny Hopping** - While mid-air, landing on a down-angled slope and jumping again within ~50ms of landing will increase velocity.

- Players can be knocked out (or _downed_) instead of killed in some situations. I haven't what these situations are but it shouldn't interfere with impressive kills. For example: getting a killing blow with a headshot should always kill.

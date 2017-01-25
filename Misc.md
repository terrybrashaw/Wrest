# Misc #

### Environment ###
Day:Night ratio is around 7:3

Nighttime atmosphere is equivalent to *Death Valley* in BF:3. Perfectly visible, blue post-process tint, brightened lights/fires.


### Sound Design ###
Guns
- 4 main sound components from a firing gun: Gunshot, gunshot echo, bullet crack and bullet whiz.
- When close enough, you *only* hear the gunshot.
- When being shot at, if you are inside hitscan range, you hear the bullet crack + gunshot echo.
- When being shot at, if you are outside hitscan range, you hear the bullet whiz + gunshot echo.
- When not being shot at, and not close enough to hear the gunshot, you only hear the gunshot echo.


### User interface ###
Player names are only visible when standing close to a player and holding your crosshair over them. Similar to CS:GO.


### Experimental ideas ###
 - A tool should be built to find any terrain geometry angled near the 'gray area' of the walkable/unwalkable range (65-75 degrees). This geometry should be rounded (making it slightly steeper or flatter) to make terrain more readable.

 - Players can be knocked out (or *downed*) instead of killed in some situations. I haven't what these situations are but it shouldn't interfere with impressive kills. For example: getting a killing blow with a headshot should always kill.

 - I'd like to explore the concept of food items being the main method of healing. There would be a different food type that drops from each mob that can be eaten raw, cooked, or combined with other items to create more exotic food. Each food item would have it's own advantage.

 - Shallow lakes, about a foot deep. Used for fishing; players can set fish traps to 'farm' fish. Players can drink from them to restore health.

 - When a player is killed, instead of turning their player model into a ragdoll, they could be broken up into vertices and disintegrate. The vertices at the location of the killing blow would expand and travel in the same trajectory as the projectile that caused the killing blow. So a fatal headshot would cause the head to 'explode' while the rest of the body disintegrates in-place almost.

 - In towns, there should be interactable objects to draw attention of players from a large distance. For example: a bell in a tower you can ring.

### End-game possibilities ###
Battle Royale:
 - Before a server-wipe the server goes into a Battle Royale.
 - Harmful gas closes in on a randomly selected bunker over a period of 15-20 minutes
 - Last player alive wins.


### Things to keep in mind ###
Keep walls flat (https://youtu.be/kapUHDkeCE8)
ESP Honeypot
Resin


### Server settings ###
The server decides which languages are allowed.

### Removed ###
- **Bunny Hopping** - While mid-air, landing on a down-angled slope and jumping again within ~50ms of landing will increase velocity.

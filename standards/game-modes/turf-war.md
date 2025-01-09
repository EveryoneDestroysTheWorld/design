# Turf War
> *"Wreck the stage and win!"*
> <br />– Entro

**Turf War** is a [game mode](./) where the player or team that destroys the most wins the game. 

## Archetypes
### Archetype usage
All [archetypes](/standards/inventory/archetypes) are enabled for this game mode. 

### Default archetype
The archetype that the contestant had in the lobby will be their default archetype. If the contestant did not choose an archetype in the lobby or no archetype can be found, the player will not have a default archetype; so, they should choose one during the round.

### Swapping archetypes 
Any active contestants can swap their current archetypes at any time. Contestants are usually restricted to the archetypes that they own; however, round rules take precedent. 

## Dashing
If a contestant has a specific amount of stamina, they can dash in a direction by pressing a movement button (left, right, up, or down) twice. The contestant will quickly move in a specific direction; however, this will somewhat reduce the contestant's current stamina.

## Bots
### Bots as interim contestants
If a qualified player leaves mid-round, then a bot will replace the player. The bot will have the same stats, archetypes, and items of the player at the time of their departure. If the player rejoins the round, the bot will disappear; however, the player will get the last stats of the bot.

### Bot personalities
Bots will be randomly assigned a personality that will define how they interact with the game. 
| Personality | Description |
| :- | :- |
| Aggressive | The bot will try to deal as much damage as possible at any cost, strategically switching from archetypes to items. Support actions and items are a low priority; they will only heal themselves if they are in a safe space or doing nothing for a while. If there is a teammate in the way of an enemy, the bot will push through. For example, if a bot has a gun that can pierce through a character, the bot is willing to take a shot if it means damaging a rival. The bot will attack anyone who attacks them, and will hunt them down. 
| Friend | The bot will choose an ally to stick by and support them whenever possible.
| Independent | The bot wil
| Mischievous | The bot typically focuses on causing structure damage, but they occasionally attack their own team. Support actions might be used on the bot or on a rival. Mischievous bots won't go out of their way to kill their teammates, but they may be the killing shot if they're at 1 HP. The bot will attack anyone who attacks them.
| Pyromaniac | Bombs! Rockets! Mines! This bot prioritizes anything that explodes and anyone they can set on fire. They prefer damaging large structures and groups, but small parts and individuals are fine too. Support actions and items are deprioritized, but if they get them, they will use them personally or use them when they get close to an ally. If bot is in a safe space for a specific amount of time, they may quickly switch to a support archetype to heal themselves, then swap back to another explosive archetype.
| Wildcard | The bot randomly chooses one of these personalities at random times that may or may not be helpful. 

### Bot skill level
A random skill level ranging from 65 to 95 is assigned to the bot when they are created.

### Bot accuracy with ranged weapons
A bot's accuracy with a ranged weapon will be determined by adding their skill level to a random number ranging from -5 to 5. Thus, the bot's accuracy can range from 60% to 100%. 

## Downed contestants
### Definition of "downed contestants"
If a contestant's current health drops to 0, they will be "downed". 

### Archetype restrictions for downed contestants
If a contestant is downed, they cannot swap their archetype until they are revived.

### Damage restrictions for downed contestants
While downed, contestants usually cannot take or deal damage to anything or anyone.

### Reviving downed contestants
Any non-downed contestant can revive a downed contestant, even if they are not on the same team.

## Friendly fire
Friendly fire, or attacking team members, is allowed by default. 

## Destroyed parts
### Definition of "destroyed parts"
If a part's current durability level reaches 0, the part will be marked as "destroyed". Parts without a durability level cannot be destroyed.

### Damage restrictions for destroyed parts
Once a part is destroyed, the part cannot take anymore damage.

### Repairing destroyed parts
Non-downed contestants can repair any destroyed part by default, including parts that have been destroyed by their own team. Once repaired, the part will lose its "destroyed" status and recover its durability.

## Results screen
The results screen will be shown at the end of the match. It will show which teams won and lost, the final destruction distribution, and all [contestant leaderboard stats](#leaderboard-statistics). From this screen, the player can ask for a rematch with the same participants or return to the lobby. Players who approve rematch requests will be queued together in a new match, while the players who refuse the request will stay behind. Bots instantly accept rematch requests.

## Statistics
### Heads-up display statistics
* Current health
* Base health, or an indicator if the current health value is different.
* Current stamina
* Base stamina, or an indicator if the current stamina value is different.
* Effects

### Leaderboard statistics
* Icon
* Display name (if applicable)
* Username
* Current archetype
* Count of destroyed parts
* Count of repaired parts 
* Count of knockouts
* Count of assisted knockouts
* Count of wipeouts

## Overtime
In case of a tie when the round ends, overtime will be activated. Overtime will end when another part is destroyed or repaired. 

## No contest
"No contest" is a round outcome that happens only if the round stops due to an error or there are no players in the server at a time after the round starts.

<!-- 
## Activity recording
Contestant and game mode activity should be recorded and stored for review after the round ends. The following attributes should be recorded:
* Contestant character position and orientation changes 
* Contestant health and stamina assignments changes 
* Contestant effect changes
* Contestant archetype ID changes
* Player connects and disconnects
* Bot personality assignments and changes
* Action usages 
* Item usages
-->

# Bots in Turf War
## Bots as interim contestants
If a qualified player leaves mid-round, then a bot will replace the player. The bot will have the same stats, archetypes, and items of the player at the time of their departure. If the player rejoins the round, the bot will disappear; however, the player will get the last stats of the bot.

## Bot personalities
Bots will be randomly assigned a personality that will define how they interact with the game. 
| Personality | Description |
| :- | :- |
| Aggressive | The bot will try to deal as much damage as possible at any cost, strategically switching from archetypes to items. Support actions and items are a low priority; they will only heal themselves if they are in a safe space or doing nothing for a while. If there is a teammate in the way of an enemy, the bot will push through. For example, if a bot has a gun that can pierce through a character, the bot is willing to take a shot if it means damaging a rival. The bot will attack anyone who attacks them, and will hunt them down. 
| Assistant | The bot will choose an ally to stick by and support them whenever possible. Their priority is destruction, but they will attack anyone who attacks their leader.
| Mischievous | The bot typically focuses on causing structure damage, but they occasionally attack their own team. Support actions might be used on the bot or on a rival. Mischievous bots won't go out of their way to kill their teammates, but they may be the killing shot if they're at 1 HP. The bot will attack anyone who attacks them.
| Ninja | The bot prioritizes silent archetypes and items that deal the most damage to characters. They will try to sneak up on their enemies, maybe try to confuse them, and take them out in the shadows.
| Pyromaniac | Bombs! Rockets! Mines! This bot prioritizes anything that explodes and anyone they can set on fire. They prefer damaging large structures and groups, but small parts and individuals are fine too. Support actions and items are deprioritized, but if they get them, they will use them personally or use them when they get close to an ally. If bot is in a safe space for a specific amount of time, they may quickly switch to a support archetype to heal themselves, then swap back to another explosive archetype.
| Wildcard | The bot randomly chooses one of these personalities at random times that may or may not be helpful. 

## Bot skill level
A random skill level ranging from 65 to 95 is assigned to the bot when they are created.

## Bot accuracy with ranged weapons
A bot's accuracy with a ranged weapon will be determined by adding their skill level to a random number ranging from -5 to 5. Thus, the bot's accuracy can range from 60% to 100%. 
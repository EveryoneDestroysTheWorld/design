# Main place
The main place should only be used as a load balancer.

## Preloading
This is the perfect time for the game to preload core assets if possible.

## Teleporting
After preloading assets, the place should teleport the player where they need to be. Listed from high priority to low priority, below are the following conditions and locations.

| Condition | Teleport location |
| :- | :- |
| The player was in a Turf War round that is active and the player is not currently restricted from the game mode. | Teleport to [Turf War](/standards/game-modes/turf-war.md) private server. |
| One of the player's friends are in the [Arena](/standards/game-modes/arena.md). | Teleport to the specific Arena server that the friend is in. | 
| The player joined the game. | Teleport to any Arena public server. | 
# Saving stages
## Zones
If there is an active part in the [action zone](./building.md#zones), the player may save the stage. Parts that are in the visible zone are also saved and accessible to players during matches. Parts in the invisible zone are not saved.

## Progress indicator
There should be a progress indicator that shows the player how far the game is into the saving process. 

## Stage metadata
After saving a new stage, the stage will be associated with a unique ID and appear in the owner's stage list. At this point, the stage creator will be able to create and modify a stage name and a description. The name and description should be restricted to a reasonable character limit. Stage creators can change the name and description of their stages at any time.

> [!IMPORTANT]
> Remember to that the user text is [filtered by Roblox](https://create.roblox.com/docs/reference/engine/classes/Chat#FilterStringForBroadcast). Unfiltered user input could cause [service disruption](https://create.roblox.com/docs/ui/text-filtering).

## Autorecovery save
The game should provide the player with an option to autosave their stage after a specified interval or before risky actions that may cause the player to disconnect from the server.

## Save locks
To prevent save conflicts, the game should lock a stage while its being saved. This means that another server should not be able to save over the data. After the save completes, the save lock should be cleared. If there is a save lock present when the player rejoins the game, the stage should be reverted and the save lock should be removed.

## Warnings
The game should warn the player to stay in the game when they see the saving symbol on their screen. If the player leaves during the process, the game will attempt to continue saving; however, there is a chance that it may fail and data could become corrupted. 
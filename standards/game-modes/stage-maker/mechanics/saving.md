# Saving stages
## Zones
If there is an active part in the [action zone](./building.md#zones), the player may save the stage. Parts that are in the visible zone are also saved and accessible to players during matches. Parts in the invisible zone are not saved.

## Progress indicator
There should be a progress indicator that shows the player how far the game is into the saving process. 

## Metadata assignments
After saving a new stage, the stage will be associated with a unique ID and appear in the owner's stage list. At this point, the owner will be able to create and modify a stage name and a description that complies with [Roblox's filters](https://create.roblox.com/docs/reference/engine/classes/Chat#FilterStringForBroadcast).

## Autosaving
The game should provide the player with an option to autosave their stage after a specified amount of time or before risky actions that may cause the player to disconnect from the server.

## Save locking
To prevent save conflicts, the game should lock a stage while its being saved. This means that another server should not be able to save over the data. After the save completes, the save lock should be cleared. 

## Warnings
The game should warn the player to stay in the game when they see the saving symbol on their screen. If the player leaves during the process, the game will attempt to continue saving; however, there is a chance that it may fail and data could become corrupted. If there is a [save lock](#save-locking) present when the player rejoins the game, the stage should be reverted and the save lock should be removed.

> [!NOTE]
> [Servers stay up for a maximum of 30 seconds after the player leaves](https://create.roblox.com/docs/reference/engine/classes/DataModel#BindToClose), so the game may complete saving too late.
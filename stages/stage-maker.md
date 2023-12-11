# Stage Maker
When entering the Stage Maker, the player must be notified that they will give an irrevocable license to Beastslash that allows the company to use the stage for free. This will prevent DMCA takedowns for player-created stages. 

## Saving
If there is an active part in the safe zone, the player may save the stage. Parts that are in the action-safe zone will be saved and accessible to players during matches. Parts are outside the action-safe zone, but in the visible zone will not be accessible to players, but will be saved and shown to players during matches. Parts that are too far away from the safe zone will be deleted.

There should be a progress bar that shows the player how far the game is into the saving process. 90% should be turning the parts into packages and 10% should be saving those packages to datastores.

After saving a new stage, the stage will be associated with a [random UUID](https://create.roblox.com/docs/reference/engine/classes/HttpService#GenerateGUID) and appear in the players' stage list. Player will be able to create a stage name and a description that abides by the [Roblox filters](https://create.roblox.com/docs/reference/engine/classes/Chat#FilterStringForBroadcast), and enable autosaving on the stage.

The game should warn the player to stay in the game when they see the saving symbol on their screen. If the player leaves during the process, the game will attempt to continue saving; however, there is a chance that it may fail and data could become corrupted. [Servers stay up for a maximum of 30 seconds after the player leaves.](https://create.roblox.com/docs/reference/engine/classes/DataModel#BindToClose), so the game may complete saving too late.

## Loading
Players can load stages from the arena or while they are editing a stage. If the player is editing a stage, the game will ask the player if they would like to save the stage before leaving.

Once the player enters the Stage Maker, the stage will begin creating instances based on the stage's save data. If a part could not be re-created due to a corruption or a game update, the player should be notified. There should be a loading bar that shows how far the game is into the loading process based on loaded instances and total instances.

## Deleting
Stage creators may delete their stages at any time. Stage metadata (name, description, etc.) and instance data will be deleted, but the player ratings and reviews related to the stage will remain.

If the player deletes the current stage they are in, they will be teleported back to the arena.
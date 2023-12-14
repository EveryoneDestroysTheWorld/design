# Stage Maker
When entering the Stage Maker, the player must be notified that they will give an irrevocable license to Beastslash that allows the company to use the stage for free. This will prevent players from sending DMCA takedown requests for their stages. 

## Building
Stage creators can build their stages with parts. The following part properties are modifiable:
* Color
* CastShadow
* Material
* Reflectance
* Transparency (max: 0.8)
* Size
* CFrame (Position, Orientation)
* Shape
* BackSurface
* BottomSurface
* FrontSurface
* LeftSurface
* RightSurface
* TopSurface

The player can also change the part's durability, which defines how much damage the part can take before getting "wrecked". 

### Smooth modeling
The player can union, negate, intersect, and separate parts. 

### Action history
The player can undo and redo recent actions. When the player undoes something and does a new action, the redo history will be deleted.

### Zones
<table>
  <thead>
    <tr>
      <th align="left">Zone name</th>
      <th align="left">Zone description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Action zone</td>
      <td>Players can access this zone normally.</td>
    </tr>
    <tr>
      <td>Visible zone</td>
      <td>Players can see this zone, but they can't access it normally. The stage creator can make the arena stands invisible to players to give them more creativity over the layout.</td>
    </tr>
    <tr>
      <td>Invisible zone</td>
      <td>Players cannot see or access this zone.</td>
    </tr>
</table>

## Navigation
The player can fly around the stage by pressing a specific button. The player can turn it off by pressing the same button. 

## Saving
If there is an active part in the safe zone, the player may save the stage. Parts that are in the action-safe zone will be saved and accessible to players during matches. Parts are outside the action-safe zone, but in the visible zone will not be accessible to players, but will be saved and shown to players during matches. Parts that are too far away from the safe zone will be deleted.

There should be a progress bar that shows the player how far the game is into the saving process. 90% should be turning the parts into packages and 10% should be saving those packages to datastores.

After saving a new stage, the stage will be associated with a [random UUID](https://create.roblox.com/docs/reference/engine/classes/HttpService#GenerateGUID) and appear in the players' stage list. Player will be able to create a stage name and a description that abides by the [Roblox filters](https://create.roblox.com/docs/reference/engine/classes/Chat#FilterStringForBroadcast), and enable autosaving on the stage.

The game should warn the player to stay in the game when they see the saving symbol on their screen. If the player leaves during the process, the game will attempt to continue saving; however, there is a chance that it may fail and data could become corrupted. [Servers stay up for a maximum of 30 seconds after the player leaves.](https://create.roblox.com/docs/reference/engine/classes/DataModel#BindToClose), so the game may complete saving too late.

## Loading
Players can load stages from the arena or while they are editing a stage. If the player is editing a stage, the game will ask the player if they would like to save the stage before leaving.

Once the player enters the Stage Maker, the stage will begin creating instances based on the stage's save data. If a part could not be re-created due to a corruption or a game update, the player should be notified. There should be a loading bar that shows how far the game is into the loading process based on loaded instances and total instances.

## Testing
All collaborators may test a stage from the arena without jury or Beastslash approval. Only collaborators with the Editor permission or higher may test a stage from the Stage Maker.

Testers may test stages alone, with bots, or with other players. They may also change the round settings to how they see fit. The testers may leave the round at any time without a penalty.

## Publishing
### Access
After the stage owner saves the stage for the first time, they may choose to publish their stage. Collaborators with admin access to the stage can publish it. 

### Jury
#### Selection
After the stage owner publishes the stage, a jury will review it. Players who have at least played ten matches may become jurors. Stage collaborators cannot be jury members. Beastslash community staff will have the option to override the jury.

#### Review and voting
After the jurors finish reviewing, they may vote on whether the stage should be played by people outside of the jury. After a stage gets ten votes, the game will determine what to do next. 

<table>
  <thead>
    <tr>
      <th align="left">Approval rate</th>
      <th align="left">Decision</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>70% or higher</td>
      <td>The stage is approved, will be added to the default stage list, and will be removed from the review center. Beastslash community staff will also be notified.</td>
    </tr>
    <tr>
      <td>50% – 69%</td>
      <td>The stage will remain on the review center until it meets another criteria.</td>
    </tr>
    <tr>
      <td>Less than 50%</td>
      <td>The stage is rejected and will be removed from the review center.</td>
    </tr>
  </tbody>
</table>

### Unpublishing
The stage owner may unpublish their stage at any time. Replays will be unavailable unless the stage owner publishes their stage again.

If a stage owner wants to publish their stage again, they can skip the jury as long as they have not made any changes to their stage. If the stage owner has made changes and publishes their stage, they will have to go through the jury process again. Furthermore, all replays related to the stage will be deleted upon stage approval.

## Collaborating
After the stage owner saves their stage for the first time, they may add collaborators to help them. 

### Credits
Before every match, the player will get a good view of the stage. While this happens, the stage owner's name will appear by default; however, anyone with Manager access can change the name shown. This can be helpful if the stage was created by a named team or a group of folks. Credits should not determined by access levels.

### Managing collaborators
The stage owner and anyone with Manager access can manage the collaborator list by pressing a specific button in the top bar.

<table>
  <thead>
    <tr>
      <th align="left">Access level</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Tester</td>
      <td>The player can test the stage from the lobby in Practice Mode. They may give feedback directly to the creator.</td>
    </tr>
    <tr>
      <td>Editor</td>
      <td>The player has Tester access in addition to being able to manage the stage's build data.</td>
    </tr>
    <tr>
      <td>Manager</td>
      <td>The player has Editor access in addition to being able to manage the stage's collaborators and metadata. They may also publish the stage on behalf of the owner.</td>
    </tr>
    <tr>
      <td>Admin</td>
      <td>The player has Manager access in addition to being able to delete the stage.</td>
    </tr>
  </tbody>
</table>

## Deleting
Stage creators may delete their stages at any time. Stage metadata (name, description, etc.) and instance data will be deleted, but the player ratings and reviews related to the stage will remain.

If the player deletes the current stage they are in, they will be teleported back to the arena.

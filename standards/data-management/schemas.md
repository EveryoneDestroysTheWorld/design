<!-- # Schemas
<table>
  <thead>
    <tr>
      <th align="left">Datastore name</th>
      <th align="left">Ordered?</th>
      <th align="left">Datastore key</th>
      <th align="left">Datastore value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>JuryReviews</td>
      <td>No</td>
      <td>
        <code>juryReviewID</code>
      </td>
      <td>
        <code>JuryReviewObject</code>
      </td>
    </tr>
    <tr>
      <td>ModifiedItems</td>
      <td>No</td>
      <td>
        <code>modifiedItemID</code>
      </td>
      <td>
        <code>ModifiedItemObject</code>
      </td>
    </tr>
    <tr>
      <td>Servers</td>
      <td>No</td>
      <td>
        <code>serverID</code>
      </td>
      <td>
        <code>ServerMetadataObject</code>
      </td>
    </tr>
    <tr>
      <td>
        ServerPlayers/<code>serverID</code>
      </td>
      <td>No</td>
      <td>
        <code>playerID</code>
      </td>
      <td>
        A list of <code>ServerPlayerMetadataObject</code>
      </td>
    </tr>
    <tr>
      <td>
        Players
      </td>
      <td>No</td>
      <td>
        <code>playerID</code>
      </td>
      <td>
        <code>PlayerMetadataObject</code>
      </td>
    </tr>
    <tr>
      <td>
        PrivilegedActions
      </td>
      <td>No</td>
      <td>
        <code>actionID</code>
      </td>
      <td>
        <code>PrivilegedActionObject</code>
      </td>
    </tr>
    <tr>
      <td>
        PrivilegedActionOrder
      </td>
      <td>Yes</td>
      <td>
        <code>actionID</code>
      </td>
      <td>
        The current time in seconds.
      </td>
    </tr>
    <tr>
      <td>Rounds</td>
      <td>No</td>
      <td>
        <code>roundID</code>
      </td>
      <td>
        <code>RoundMovementObject</code>
      </td>
    </tr>
    <tr>
      <td>RoundMovements/<code>roundID</code></td>
      <td>No</td>
      <td>
        <code>playerID</code>/<code>1...n</code>
      </td>
      <td>
        A list of HumanoidRootPart CFrame components, maximum 4 million characters
      </td>
    </tr>
    <tr>
      <td>RoundItemActs/<code>roundID</code></td>
      <td>No</td>
      <td>
        <code>playerID</code>/<code>1...n</code>
      </td>
      <td>
        A list of <code>ItemActionObject</code>, maximum 4 million characters
      </td>
    </tr>
    <tr>
      <td>Stages</td>
      <td>No</td>
      <td>
        <code>stageID</code>
      </td>
      <td>
        <code>StageMetadataObject</code>
      </td>
    </tr>
    <tr>
      <td>StageInstances</td>
      <td>No</td>
      <td>
        <code>stageID</code>/<code>1...n</code>
      </td>
      <td>
        A list of <code>StageInstanceInfo</code>, maximum 4 million characters
      </td>
    </tr>
  </tbody>
</table>

## JSON objects
### `ModifiedItemObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>name</td>
      <td>
        The item name.
      </td>
    </tr>
    <tr>
      <td>description</td>
      <td>
        The item description.
      </td>
    </tr>
    <tr>
      <td>modifications</td>
      <td>
        A list of modifications that the item has.
      </td>
    </tr>
  </tbody>
</table>

### `PrivilegedActionObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>actorID</td>
      <td>
        The actor's ID.
      </td>
    </tr>
    <tr>
      <td>permission</td>
      <td>
        The <a href="../player-support/permissions.md">permission</a> used in the action.
      </td>
    </tr>
    <tr>
      <td>changes?</td>
      <td>
        A list of <code>PrivilegedActionChangeObject</code>, if applicable.
      </td>
    </tr>
    <tr>
      <td>tick</td>
      <td>
        A tick of when the action happened.
      </td>
    </tr>
    <tr>
      <td>targetID</td>
      <td>
        An ID of an applicable object.
      </td>
    </tr>
    <tr>
      <td>reason?</td>
      <td>
        A reason, if applicable.
      </td>
    </tr>
    <tr>
      <td>tickDuration</td>
      <td>Ticks that the server lasted.</td>
    </tr>
  </tbody>
</table>

### `PrivilegedActionChangeObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>newValue?</td>
      <td>
        New key value.
      </td>
    </tr>
    <tr>
      <td>oldValue?</td>
      <td>
        Old key value.
      </td>
    </tr>
    <tr>
      <td>key</td>
      <td>
        Key name.
      </td>
    </tr>
  </tbody>
</table>

### `ItemActionObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>tick</td>
      <td>Tick since round start.</td>
    </tr>
    <tr>
      <td>itemID</td>
      <td>The ID of the item used.</td>
    </tr>
    <tr>
      <td>lookVector</td>
      <td>The look vector CFrame of the mouse.</td>
    </tr>
  </tbody>
</table>

### `JurorResponseObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>jurorID</td>
      <td>Tick since round start.</td>
    </tr>
    <tr>
      <td>timeMade</td>
      <td>Time in seconds when this response was sent.</td>
    </tr>
    <tr>
      <td>timeUpdated?</td>
      <td>Time in seconds when this response was updated.</td>
    </tr>
    <tr>
      <td>reason?</td>
      <td>A reason for this response.</td>
    </tr>
    <tr>
      <td>decision</td>
      <td>
        An integer depending on the juror's decision.
        <ol>
          <li>Approve</li>
          <li>Deny</li>
          <li>Skip</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

### `JuryReviewObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>stageID</td>
      <td>The ID of the stage in question.</td>
    </tr>
    <tr>
      <td>timeOpened</td>
      <td>Tick since round start.</td>
    </tr>
    <tr>
      <td>timeClosed</td>
      <td>The ID of the item used.</td>
    </tr>
    <tr>
      <td>responses</td>
      <td>A list of `JurorResponseObject`.</td>
    </tr>
  </tbody>
</table>

### `PlayerMetadataObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>roleID</td>
      <td>Timestamp of the server's opening.</td>
    </tr>
    <tr>
      <td>inventory</td>
      <td>
        <code>InventoryMetadataObject</code>
      </td>
    </tr>
    <tr>
      <td>permissions</td>
      <td>
        <code>PermissionOverrideObject</code>
      </td>
    </tr>
    <tr>
      <td>settings</td>
      <td>
        <code>PlayerSettingsOverrideObject</code>
      </td>
    </tr>
    <tr>
      <td>title?</td>
      <td>
        The player's title.
      </td>
    </tr>
    <tr>
      <td>timeFirstPlayed</td>
      <td>
        The time the player first joined the game.
      </td>
    </tr>
    <tr>
      <td>timeLastPlayed</td>
      <td>
        The latest time the player joined the game.
      </td>
    </tr>
  </tbody>
</table>

### `PermissionOverrideObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>allow</td>
      <td>A list of <code>PermissionManagementOverrideObject</code></td>
    </tr>
    <tr>
      <td>deny</td>
      <td>A list of permissions.</td>
    </tr>
  </tbody>
</table>

### `PermissionManagementOverrideObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>permission</code></td>
      <td>A permission management level.</td>
    </tr>
  </tbody>
</table>

### `PlayerSettingsOverrideObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>settingName</code></td>
      <td>The setting value.</td>
    </tr>
  </tbody>
</table>

### `RoundMetadataObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>participantIDs</td>
      <td>A list of player IDs.</td>
    </tr>
    <tr>
      <td>stageID</td>
      <td>The stage's ID.</td>
    </tr>
    <tr>
      <td>serverID</td>
      <td>The round's server ID.</td>
    </tr>
    <tr>
      <td>tickDuration</td>
      <td>The number of ticks that the round lasted.</td>
    </tr>
    <tr>
      <td>tickStarted</td>
      <td>Tick of the round start.</td>
    </tr>
    <tr>
      <td>type</td>
      <td>
        An integer, depending on the round's type.
        <ol>
          <li>Turf War</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

### `ServerMetadataObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>tickStarted</td>
      <td>Timestamp of the server's opening.</td>
    </tr>
    <tr>
      <td>tickDuration</td>
      <td>Ticks that the server lasted.</td>
    </tr>
  </tbody>
</table>

### `ServerPlayerMetadataObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>tickJoined</td>
      <td>Player join timestamp.</td>
    </tr>
    <tr>
      <td>tickDuration</td>
      <td>Player join duration in seconds.</td>
    </tr>
  </tbody>
</table>

### `StageInstanceObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>name</td>
      <td>The part's name.</td>
    </tr>
    <tr>
      <td>color</td>
      <td>The part's hex color code.</td>
    </tr>
    <tr>
      <td>size</td>
      <td>An array of part dimensions.</td>
    </tr>
    <tr>
      <td>cframe</td>
      <td>An array of CFrame components.</td>
    </tr>
    <tr>
      <td>castShadow?</td>
      <td>1, if CastShadow is enabled on this part.</td>
    </tr>
    <tr>
      <td>material?</td>
      <td>A Material enum value, if this part isn't plastic.</td>
    </tr>
    <tr>
      <td>reflectance?</td>
      <td>The part's reflectance level, if it isn't 0.</td>
    </tr>
    <tr>
      <td>transparency?</td>
      <td>The part's transparency level, if it isn't 0.</td>
    </tr>
    <tr>
      <td>shape?</td>
      <td>A PartType enum value, if this part isn't a block.</td>
    </tr>
    <tr>
      <td>backSurface?</td>
      <td>A SurfaceType enum value, if this part isn't smooth.</td>
    </tr>
    <tr>
      <td>bottomSurface?</td>
      <td>A SurfaceType enum value, if this part isn't smooth.</td>
    </tr>
    <tr>
      <td>frontSurface?</td>
      <td>A SurfaceType enum value, if this part isn't smooth.</td>
    </tr>
    <tr>
      <td>leftSurface?</td>
      <td>A SurfaceType enum value, if this part isn't smooth.</td>
    </tr>
    <tr>
      <td>rightSurface?</td>
      <td>A SurfaceType enum value, if this part isn't smooth.</td>
    </tr>
    <tr>
      <td>topSurface?</td>
      <td>A SurfaceType enum value, if this part isn't smooth.</td>
    </tr>
  </tbody>
</table>

### `StageMetadataObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>creatorIDs</td>
      <td>The IDs of the stage's creators. This should not be used for permissions.</td>
    </tr>
    <tr>
      <td>juryActionID?</td>
      <td>A <code>JuryActionObject</code> ID. Only present for user-published stages.</td>
    </tr>
    <tr>
      <td>staffActionID?</td>
      <td>A <code>StaffActionObject</code> ID. Only present for stages that Beastslash flags.</td>
    </tr>
    <tr>
      <td>members</td>
      <td>A list of <code>StageMemberObject</code>.</td>
    </tr>
    <tr>
      <td>stageName</td>
      <td>The stage's name.</td>
    </tr>
    <tr>
      <td>timeCreated</td>
      <td>Time in seconds when the stage was created.</td>
    </tr>
    <tr>
      <td>timeCreated</td>
      <td>Time in seconds when the stage was last updated.</td>
    </tr>
  </tbody>
</table>

### `StageMemberObject`
<table>
  <thead>
    <tr>
      <th align="left">Object key</th>
      <th align="left">Object value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>id</td>
      <td>The player ID.</td>
    </tr>
    <tr>
      <td>role</td>
      <td>
        An integer depending on the player's role.
        <ol>
          <li>Admin</li>
          <li>Editor</li>
          <li>Player</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>

## Variables
<table>
  <thead>
    <tr>
      <th align="left">Variable name</th>
      <th align="left">Variable description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code>serverID</code>
      </td>
      <td>The server's JobId. Can be found with <code>game.JobId</code></td>
    </tr>
    <tr>
      <td>
        <code>m...n</code>
      </td>
      <td>A number depending on the previous item. Starts at <code>m</code> and ends at <code>n</code>.</td>
    </tr>
  </tbody>
</table>
 -->

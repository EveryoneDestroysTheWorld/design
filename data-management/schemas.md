# Schemas
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
        <code>playerID</code>/<code>1...n</code>
      </td>
      <td>
        A list of <code>ServerPlayerMetadataObject</code>
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
        <code>stageID</code>/<code>1...n</code>
      </td>
      <td>
        <code>StageMetadataObject</code>
      </td>
    </tr>
  </tbody>
</table>

## JSON objects
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


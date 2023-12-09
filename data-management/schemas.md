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
        A list of HumanoidRootPart CFrame components, maximum 4 million characters per item
      </td>
    </tr>
  </tbody>
</table>

## JSON objects
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
      <td>duration</td>
      <td>The number of seconds that the round lasted.</td>
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
      <td>timeStarted</td>
      <td>Timestamp of the round start time.</td>
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
      <td>timeStarted</td>
      <td>Timestamp of the server's opening.</td>
    </tr>
    <tr>
      <td>duration</td>
      <td>The number of seconds that the server lasted.</td>
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
      <td>joinTime</td>
      <td>Player join timestamp.</td>
    </tr>
    <tr>
      <td>duration</td>
      <td>Player join duration in seconds.</td>
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


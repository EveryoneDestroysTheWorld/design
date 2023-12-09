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
        <code>ServerPlayerMetadataObject</code>
      </td>
    </tr>
  </tbody>
</table>

## JSON objects
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
      <td>openTime</td>
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


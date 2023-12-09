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
  </tbody>
</table>


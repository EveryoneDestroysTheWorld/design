# User interfaces
## Player profile window
### Header
The header is always shown.

<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Type</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Close</td>
      <td>Button</td>
      <td>Closes the player profile window.</td>
    </tr>
    <tr>
      <td>Back</td>
      <td>Button</td>
      <td>Goes to the previous page. Only shows if the player went to another profile.</td>
    </tr>
    <tr>
      <td>Spectate</td>
      <td>Button</td>
      <td>Only available when the player is in a match and for players with permission to spectate.</td>
    </tr>
    <tr>
      <td>Report</td>
      <td>Button</td>
      <td>Opens the report menu.</td>
    </tr>
    <tr>
      <td><code>username</code></td>
      <td>Text</td>
      <td><code>username</code> should be replaced with the player's username.</td>
    </tr>
  </tbody>
</table>

### Overview
The overview view is the default view. 

<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Type</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Player pose</td>
      <td>Model</td>
      <td>A 3D model visualization of the player's character. This will be the background of the profile.</td>
    </tr>
    <tr>
      <td><code>displayName</code></td>
      <td>Text</td>
      <td><code>displayName</code> is the player's display name.</td>
    </tr>
    <tr>
      <td><code>title</code></td>
      <td>Text</td>
      <td><code>title</code> is the player's title.</td>
    </tr>
    <tr>
      <td>Country flag</td>
      <td>Image</td>
      <td>A small icon of the player's country flag.</td>
    </tr>
    <tr>
      <td>Stats</td>
      <td>Button</td>
      <td>Opens the stats view.</td>
    </tr>
    <tr>
      <td>Records</td>
      <td>Button</td>
      <td>Opens the records view.</td>
    </tr>
    <tr>
      <td>Stages</td>
      <td>Button</td>
      <td>Opens the stages view.</td>
    </tr>
  </tbody>
</table>

### Stats view
The stats view will be a list of 

### Records view
The records view will show a list of all recorded matches. 

<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Type</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>result</code></td>
      <td>Text</td>
      <td><code>result</code> could be "Win", "Lose", "Tie", or "No contest", depending on the result of the match.</td>
    </tr>
    <tr>
      <td><code>ownScore</code> – <code>rivalScore</code></td>
      <td>Text</td>
      <td><code>ownScore</code> is the number of rounds that the player won in the match, while <code>rivalScore</code> reflects the rival team's score. In case there are matches with more than two teams, then there will be more rival scores shown; however, the player's score will always be the first.</td>
    </tr>
    <tr>
      <td><code>matchStartDate</code></td>
      <td>Text</td>
      <td>The date of the match.</td>
    </tr>
    <tr>
      <td>Match ID: <code>matchID</code></td>
      <td>Text</td>
      <td><code>displayName</code> is the player's display name.</td>
    </tr>
    <tr>
      <td>Rounds</td>
      <td>Dropdown list toggle</td>
      <td>Toggles a dropdown list that shows the rounds.</td>
    </tr>
  </tbody>
</table>

#### Round item
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Type</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>result</code></td>
      <td>Text</td>
      <td><code>result</code> could be "Win", "Lose", "Tie", or "No contest", depending on the result of the match.</td>
    </tr>
    <tr>
      <td><code>ownScore</code> – <code>rivalScore</code></td>
      <td>Text</td>
      <td><code>ownScore</code> is the player's score at the end of the round, while <code>rivalScore</code> reflects the rival team's score. In case there are matches with more than two teams, then there will be more rival scores shown; however, the player's score will always be the first.</td>
    </tr>
    <tr>
      <td><code>participantImages</code></td>
      <td>Buttons</td>
      <td>A photo of each round participant, separated by team. The button will lead to their profile.</td>
    </tr>
    <tr>
      <td><code>roundDuration</code></td>
      <td>Text</td>
      <td>The duration of the round.</td>
    </tr>
    <tr>
      <td>Round ID: <code>roundID</code></td>
      <td>Text</td>
      <td>The ID of the round.</td>
    </tr>
    <tr>
      <td>Watch replay</td>
      <td>Button</td>
      <td>Only shows if replay data for the round is accessible.</td>
    </tr>
  </tbody>
</table>

### Stages view
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Type</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>stageName</code></td>
      <td>Text</td>
      <td>Replaced with the name of the stage.</td>
    </tr>
    <tr>
      <td><code>stageCreatorName</code></td>
      <td>Text</td>
      <td></td>
    </tr>
    <tr>
      <td><code>stageCollaboratorImages</code></td>
      <td>Buttons</td>
      <td>Image buttons of the stage collaborators, sorted by rank, then by username. Only visible to collaborators.</td>
    </tr>
    <tr>
      <td>Edit in Stage Maker</td>
      <td>Button</td>
      <td>Only visible to collaborators.</td>
    </tr>
    <tr>
      <td></td>
      <td>Buttons</td>
      <td>A photo of each round participant, separated by team. The button will lead to their profile.</td>
    </tr>
    <tr>
      <td><code>roundDuration</code></td>
      <td>Text</td>
      <td>The duration of the round.</td>
    </tr>
    <tr>
      <td>Stage ID: <code>roundID</code></td>
      <td>Text</td>
      <td>The ID of the round.</td>
    </tr>
    <tr>
      <td>Watch replay</td>
      <td>Button</td>
      <td>Only shows if replay data for the round is accessible.</td>
    </tr>
  </tbody>
</table>

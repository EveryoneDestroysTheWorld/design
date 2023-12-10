# Permissions
## Management levels
For security reasons, the default management level for all permissions should be 0. The place owner should always have level 3 management access for every permission.

<table>
  <thead>
    <tr>
      <th align="left">Level</th>
      <th align="left">Type</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>Normal</td>
      <td>The player will have no management access.</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Audit</td>
      <td>The player or role can see everyone's level of access to this permission.</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Admin</td>
      <td>The player or role will have full management access to this permission.</td>
    </tr>
  </tbody>
</table>

## Permission groups
### Economy
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>economy.trading.initiate</code></td>
      <td>Allows the player to initiate trades.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>economy.trading.participate</code></td>
      <td>Allows the player to participate in trades.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>economy.shop.purchase</code></td>
      <td>Allows the player to purchase items and boosts from the shop.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>economy.developerProducts.purchase</code></td>
      <td>Allows the player to purchase developer products.</td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>

### Logs
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>logs.chat.view</code></td>
      <td>Allows the player to view chat logs.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>logs.juryDecisions.view</code></td>
      <td>Allows the player to view jury decision logs.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>logs.staffActions.view</code></td>
      <td>Allows the player to view staff action logs.</td>
      <td>No</td>
    </tr>
  </tbody>
</table>

### Messages
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>messages.chat.remove.own</code></td>
      <td>Allows the player to remove own chat messages.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>messages.chat.remove.others</code></td>
      <td>Allows the player to remove other players' chat messages.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>messages.chat.view.own</code></td>
      <td>Allows the player to view their own chat messages.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>messages.chat.view.others</code></td>
      <td>Allows the player to view others' chat messages</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>messages.chat.send</code></td>
      <td>Allows the player to send chat messages.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>messages.direct.send</code></td>
      <td>Allows the player to send direct messages.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>messages.direct.view.own</code></td>
      <td>Allows the player to view own direct messages</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>messages.direct.view.others</code></td>
      <td>Allows the player to view others' chat messages</td>
      <td>No</td>
    </tr>
  </tbody>
</table>

### Places
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>places.lobby.join</code></td>
      <td>Allows the player to join the lobby. If the player doesn't have this permission, they are effectively banned.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>places.stageMaker.join</code></td>
      <td>Allows the player to join the Stage Maker.</td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>

### Players
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>players.badges.grant.self</code></td>
      <td>Allows the player to grant badges to themself.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.badges.grant.others</code></td>
      <td>Allows the player to grant badges to other players.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.general.kick.self</code></td>
      <td>Allows the player to kick themself from the server.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.general.kick.others</code></td>
      <td>Allows the player to kick others from the server.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.roles.view.own</code></td>
      <td>Allows the player to view their own roles.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.roles.view.others</code></td>
      <td>Allows the player to view other players' roles.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.settings.view.own</code></td>
      <td>Allows the player to view their own settings.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>players.settings.view.others</code></td>
      <td>Allows the player to view others' settings.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.settings.manage.own</code></td>
      <td>Allows the player to manage their own settings.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>players.settings.manage.others</code></td>
      <td>Allows the player to manage others' settings.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.stats.view.own</code></td>
      <td>Allows the player to view their own statistics.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>players.stats.view.others</code></td>
      <td>Allows the player to view other players' statistics.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>players.stats.manage.own</code></td>
      <td>Allows the player to manage their own statistics.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.stats.manage.others</code></td>
      <td>Allows the player to manage other players' statistics.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>players.titles.choose.own</code></td>
      <td>Allows the player to choose their own titles.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>players.titles.choose.others</code></td>
      <td>Allows the player to choose others' titles.</td>
      <td>No</td>
    </tr>
  </tbody>
</table>

### Feedback
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>feedback.send</code></td>
      <td>Allows the player to write game feedback.</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td><code>feedback.respond</code></td>
      <td>Allows the player to respond to or close game feedback.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>feedback.delete</code></td>
      <td>Allows the player to delete game feedback.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>feedback.view</code></td>
      <td>Allows the player to view game feedback.</td>
      <td>No</td>
    </tr>
  </tbody>
</table>

### Roles
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>roles.create</code></td>
      <td>Allows the player to create roles.</td>
      <td>No</td>
    </tr>
  </tbody>
</table>

### Matches
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Description</th>
      <th align="left">Default?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>matches.general.respawn.self</code></td>
      <td>Allows the player to respawn themself, even if they are permanently dead.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.general.respawn.others</code></td>
      <td>Allows the player to respawn other players, even if they are permanently dead.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.participants.add.self</code></td>
      <td>Allows the player to add themself to a match's participant list, even if it's ongoing.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.participants.add.others</code></td>
      <td>Allows the player to add another player to a match's participant list, even if it's ongoing.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.participants.eject.self</code></td>
      <td>Allows the player to eject themself from a match's participant list.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.participants.eject.others</code></td>
      <td>Allows the player to eject another player to a match's participant list.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.rules.manage</code></td>
      <td>Allows the player to manage the round's rules without voting.</td>
      <td>No</td>
    </tr>
    <tr>
      <td><code>matches.rules.vote</code></td>
      <td>Allows the player to vote on the round's rules.</td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>

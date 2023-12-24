# Dreamstone Shop
The Dreamstone Shop is a place where players can spend their Dreamstone on items, abilities, weapons, and boosts. Be careful though: it's operated by a demon from the Greed District. If you aren't happy, you aren't getting your money back.

Players can find the shop in the arena.

## Weapons
<table>
  <thead>
    <tr>
      <th align="left">Name</th>
      <th align="left">Price</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Scatterburst</td>
      <td>TBD</td>
    </tr>
  </tbody>
</table>

## User interface
### Header
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
      <td>Goes to the previous page. Only shows if the player went to another view.</td>
    </tr>
    <tr>
      <td>Spectate</td>
      <td>Button</td>
      <td>Only available when the player is in a match and for players with permission to spectate.</td>
    </tr>
    <tr>
      <td>Dreamstone Shop</td>
      <td>Text</td>
      <td>This is the window name.</td>
    </tr>
    <tr>
      <td><code>dreamstone</code></td>
      <td>Text</td>
      <td>THe amount of Dreamstone the player has</td>
    </tr>
  </tbody>
</table>

### Overview
This is the default view.

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
      <td>Abilities</td>
      <td>Button</td>
      <td>Opens the abilities view.</td>
    </tr>
    <tr>
      <td>Items</td>
      <td>Button</td>
      <td>Opens the items view.</td>
    </tr>
    <tr>
      <td>Attachments</td>
      <td>Button</td>
      <td>Opens the attachments view.</td>
    </tr>
  </tbody>
</table>

### All views, excluding Overview
Each item, ability, and attachment will use this button template: 

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
      <td><code>itemIcon</code></td>
      <td>Image</td>
      <td>Replaced with the item icon.</td>
    </tr>
    <tr>
      <td><code>itemName</code></td>
      <td>Text</td>
      <td>Replaced with the item name.</td>
    </tr>
    <tr>
      <td><code>dreamstonePrice</code></td>
      <td>Text</td>
      <td>Replaced with the item price.</td>
    </tr>
  </tbody>
</table>

On the right side, the player may find details of the items and purchase it.

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
      <td><code>itemIcon</code></td>
      <td>Image</td>
      <td>Replaced with item icon.</td>
    </tr>
    <tr>
      <td><code>itemName</code></td>
      <td>Text</td>
      <td>Replaced with item name.</td>
    </tr>
    <tr>
      <td><code>itemPreview</code></td>
      <td>Model</td>
      <td>Replaced with a 3D model preview of the item.</td>
    </tr>
    <tr>
      <td><code>dreamstonePrice</code></td>
      <td>Text</td>
      <td>Replaced with the item price.</td>
    </tr>
    <tr>
      <td>Purchase</td>
      <td>Button</td>
      <td>Only works if the player has enough Dreamstone.</td>
    </tr>
  </tbody>
</table>

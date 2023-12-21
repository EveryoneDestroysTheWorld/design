# User interfaces
## Dreamstone Shop
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
      <td>Workshop</td>
      <td>Text</td>
      <td>This is the window name.</td>
    </tr>
  </tbody>
</table>

### Items view
This is the default view. All of the player's items will be shown on this screen. Attachments and abilities should not be shown. 

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
  </tbody>
</table>

### Selected item view
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
      <td><code>stats</code></td>
      <td>Text</td>
      <td>A list of stats will be shown.</td>
    </tr>
    <tr>
      <td><code>attachment</code></td>
      <td>Button</td>
      <td>Opens the attachments view.</td>
    </tr>
  </tbody>
</table>

### Attachments view
All compatible attachments will be shown on this view.

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
      <td><code>attachmentIcon</code></td>
      <td>Image</td>
      <td>Replaced with the item icon.</td>
    </tr>
    <tr>
      <td><code>attachmentName</code></td>
      <td>Text</td>
      <td>Replaced with the item name.</td>
    </tr>
  </tbody>
</table>

On the right side, there is a UI that gives more details on the chosen attachment.

table>
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
      <td>Replaced with a 3D model preview of the item with the attachment.</td>
    </tr>
    <tr>
      <td><code>modifiedStats</code></td>
      <td>Text</td>
      <td>Replaced with the base stats with the modifications highlighted.</td>
    </tr>
    <tr>
      <td>Attach</td>
      <td>Button</td>
      <td>Only works if the attachment is detached from the current item.</td>
    </tr>
    <tr>
      <td>Detach</td>
      <td>Button</td>
      <td>Only works if the attachment is attached from the current item.</td>
    </tr>
  </tbody>
</table>
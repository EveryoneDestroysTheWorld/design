# Player settings
The player can change a variety of settings to personalize their experience in the game. The player can access these settings through the in-game pause menu.

## Controls
<table>
  <thead>
    <th align="left">Name</th>
    <th align="left">Internal name</th>
    <th align="left">Description</th>
    <th align="left">Type</th>
    <th align="left">Default value</th>
  </thead>
  <tbody>
    <tr>
      <td>Go back one page</td>
      <td>controls.backButton</td>
      <td>Navigates to the last page in a UI.</td>
      <td>Keybind</td>
      <td>
        Keyboard: <code>Enum.KeyCode.Backspace</code>
        Gamepad: <code>Enum.KeyCode.ButtonB</code>
      </td>
    </tr>
    <tr>
      <td>Close UI</td>
      <td>
        <code>controls.closeButton</code>
      </td>
      <td>Shortcut button that closes a user interface.</td>
      <td>Keybind</td>
      <td>
        Keyboard: <code>Enum.KeyCode.End</code><br />
        Gamepad: <code>Enum.KeyCode.ButtonY</code>
      </td>
    </tr>
    <tr>
      <td>Toggle pause menu</td>
      <td>
        <code>controls.togglePauseMenuButton</code>
      </td>
      <td>Button that toggles the DemoDemons pause menu. This should not conflict with the Roblox pause menu button (currently <code>Enum.KeyCode.Escape</code>).</td>
      <td>KeyCode input</td>
      <td>
        <code>Enum.KeyCode.Pause</code>
      </td>
    </tr>
  </tbody>
</table>

## Volume
<table>
  <thead>
    <th align="left">Name</th>
    <th align="left">Internal name</th>
    <th align="left">Description</th>
    <th align="left">Type</th>
    <th align="left">Default value</th>
  </thead>
  <tbody>
    <tr>
      <td>Main volume</td>
      <td><code>volume.main</code></td>
      <td>A percentage representing the main volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Music volume</td>
      <td>
        <code>volume.music</code>
      </td>
      <td>A percentage representing the music volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Sound effect volume</td>
      <td>
        <code>volume.sfx</code>
      </td>
      <td>A percentage representing the sound effect volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Ambience volume</td>
      <td>
        <code>volume.ambience</code>
      </td>
      <td>A percentage representing the ambience volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>System message volume</td>
      <td>
        <code>volume.systemMessages</code>
      </td>
      <td>A percentage representing the system message volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Item volume</td>
      <td>
        <code>volume.items</code>
      </td>
      <td>A percentage representing the item volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Chat mention volume</td>
      <td>
        <code>volume.chatMentions</code>
      </td>
      <td>A percentage representing the chat mention volume level.</td>
      <td>Slider (0 – 1, decimals accepted)</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

## Accessibility
<table>
  <thead>
    <th align="left">Name</th>
    <th align="left">Internal name</th>
    <th align="left">Description</th>
    <th align="left">Type</th>
    <th align="left">Default value</th>
  </thead>
  <tbody>
    <tr>
      <td>Sound subtitles</td>
      <td>
        <code>accessibility.subtitles.sound.enabled</code>
      </td>
      <td>A toggle for sound subtitles. This will show the direction of each sound that plays in the player's proximity.</td>
      <td>Checkbox</td>
      <td>Enabled</td>
    </tr>
  </tbody>
</table>

## Data and privacy
<table>
  <thead>
    <th align="left">Name</th>
    <th align="left">Internal name</th>
    <th align="left">Description</th>
    <th align="left">Type</th>
    <th align="left">Default value</th>
  </thead>
  <tbody>
    <tr>
      <td>Transfer profile</td>
      <td></td>
      <td>
        Starts the <a href="../data-management/save-profiles.md#transferring-save-profiles">profile transfer process</a>.
      </td>
      <td>Button</td>
      <td></td>
    </tr>
    <tr>
      <td>Delete profile</td>
      <td></td>
      <td>
        Starts the <a href="../data-management/save-profiles.md#deleting-save-profiles">profile deletion process</a>.
      </td>
      <td>Button</td>
      <td></td>
    </tr>
  </tbody>
</table>

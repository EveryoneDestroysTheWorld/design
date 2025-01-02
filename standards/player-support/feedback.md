# Feedback screen
The **feedback screen** is a UI that allows players to submit suggestions, comments, and concerns to Beastslash. If the player would like a response from Beastslash, then the feedback will be treated as a ticket.

The player can access it from the pause menu.

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
      <td>Feedback</td>
      <td>Text</td>
      <td>This is the window name.</td>
    </tr>
    <tr>
      <td>View submitted feedback</td>
      <td>Button</td>
      <td>Opens the submissions view.</td>
    </tr>
  </tbody>
</table>

### Content view
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
      <td>What do you think about DemoDemons? Let us know here.</td>
      <td>Large text box input</td>
      <td>Replaced with the item icon.</td>
    </tr>
    <tr>
      <td>I need a response</td>
      <td>Checkbox</td>
      <td>If checked, this feedback becomes a ticket.</td>
    </tr>
    <tr>
      <td>Submit</td>
      <td>Button</td>
      <td>Only available after the player enters something in the text box.</td>
    </tr>
    <tr>
      <td>Once you press submit, we'll review your feedback to improve the game. To help us better understand, this will highlight some information about your current server and your player profile.</td>
      <td>Large text box input</td>
      <td>Replaced with the item icon.</td>
    </tr>
  </tbody>
</table>

### Submitted view
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
      <td>Thanks for sending feedback to Beastslash!</td>
      <td>Text</td>
      <td></td>
    </tr>
    <tr>
      <td>We'll get back to you soon.</td>
      <td>Text</td>
      <td>Only shows if the player checked "I need a response".</td>
    </tr>
    <tr>
      <td>Close</td>
      <td>Button</td>
      <td>Closes the UI.</td>
    </tr>
  </tbody>
</table>

### Submissions view
For each submission, there will be a button with the following children:

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
      <td><code>contentTruncated</code></td>
      <td>Text</td>
      <td>Replaced with the feedback's content.</td>
    </tr>
    <tr>
      <td><code>status</code></td>
      <td>Text</td>
      <td>Can be replaced with "Received", "Awaiting your response", "Awaiting Beastslash's response", "Investigating", or "Closed".</td>
    </tr>
  </tbody>
</table>

If the player has the `feedback.view` permission, they can view feedback from other people. From here, they can also delete the feedback if they have the `feedback.delete` permission.

### Activity view
At the bottom, the player can respond to Beastslash:

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
      <td>Message box</td>
      <td>Input box</td>
      <td></td>
    </tr>
    <tr>
      <td>Send</td>
      <td>Button</td>
      <td>Sends a message to Beastslash.</td>
    </tr>
  </tbody>
</table>

If the player has the `feedback.respond` permission, they can respond on behalf of Beastslash.
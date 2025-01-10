# Turf War
> *"Wreck the stage and win!"*
> <br />– Entro

**Turf War** is a [game mode](./) where the player or team that destroys the most wins the game. 

## Archetypes
### Eligible archetypes
All [archetypes](/standards/inventory/archetypes) are eligible for this game mode. 

### Default archetype
The archetype that the contestant had in the lobby will be their default archetype. If the contestant did not choose an archetype in the lobby or no archetype can be found, the player will not have a default archetype; so, they should choose one during the round.

### Swapping archetypes 
Any active contestants can swap their current archetypes at any time. Contestants are usually restricted to the archetypes that they own; however, round rules take precedent. 

## Items
All [items](/standards/inventory/items) are eligible for this game mode.

## Dashing
If a contestant has a specific amount of stamina, they can dash in a direction by pressing a movement button (left, right, up, or down) twice. The contestant will quickly move in a specific direction; however, this will somewhat reduce the contestant's current stamina.

## Destroyed parts
### Definition of "destroyed parts"
If a part's current durability level reaches 0, the part will be marked as "destroyed". Parts without a durability level cannot be destroyed.

### Damage restrictions for destroyed parts
Once a part is destroyed, the part cannot take anymore damage.

### Repairing destroyed parts
Non-downed contestants can repair any destroyed part by default, including parts that have been destroyed by their own team. Once repaired, the part will lose its "destroyed" status and recover its durability.

## Results screen
The results screen will be shown at the end of the match. It will show which teams won and lost, the final destruction distribution, and all [contestant leaderboard stats](#leaderboard-statistics). From this screen, the player can ask for a rematch with the same participants or return to the lobby. Players who approve rematch requests will be queued together in a new match, while the players who refuse the request will stay behind. Bots instantly accept rematch requests.

## Statistics
### Heads-up display statistics
* Current health
* Base health, or an indicator if the current health value is different.
* Current stamina
* Base stamina, or an indicator if the current stamina value is different.
* Effects

### Leaderboard statistics
* Icon
* Display name (if applicable)
* Username
* Current archetype
* Count of destroyed parts
* Count of repaired parts 
* Count of knockouts
* Count of assisted knockouts
* Count of wipeouts

## Overtime
In case of a tie when the round ends, overtime will be activated. Overtime will end when another part is destroyed or repaired. 

## No contest
"No contest" is a round outcome that happens only if the round stops due to an error or there are no players in the server at a time after the round starts.

## Forfeiting the match
The player can leave the match only if the rest of the team agrees to forfeit the match. 

### Punishments for leaving teams behind
If the player leaves the match for any reason without submitting a successful request, they can be punished by their team at the end of the round.

* **Temporary match ban:** The player can't matchmake until a timer runs out.
* **Purgatory match:** The player can only matchup with others who left early.
* **Rewards tax:** The player can freely matchup, but half of their winnings will be taxed and given to the team members.
* **Nothing:** The team decides not to act on it, acquitting the player. 

<!-- ## Ranks
Ranks will be based on [OpenSkill](https://devforum.roblox.com/t/openskill-a-skill-based-rating-system-for-matchmaking/1571168). Ranks will be hidden from the players and will only be used for matchmaking. -->

<!-- ## Round rules
A player may vote to adjust the current server’s game rules unless the server is a VIP server. If it is a VIP server, then the server owner and designated server admins will have access to immediately change the rules to their desire.

Rule changes will take effect in the next round.

<table>
  <thead>
    <tr>
      <th align="left">Rule name</th>
      <th align="left">Restraint</th>
      <th align="left">Default value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Round time</td>
      <td>Minimum 30 seconds</td>
      <td>3 minutes</td>
    </tr>
    <tr>
      <td>Special round chance</td>
      <td>Minimum 0%</td>
      <td>25%</td>
    </tr>
    <tr>
      <td>Environmental hazards</td>
      <td>Toggle</td>
      <td>On</td>
    </tr>
    <tr>
      <td>Friendly fire</td>
      <td>Toggle</td>
      <td>Off</td>
    </tr>
    <tr>
      <td>Out-of-bounds action</td>
      <td>Selctor: Self-destruct or respawn at safe zone</td>
      <td>Self-destruct</td>
    </tr>
    <tr>
      <td>Instant respawning</td>
      <td>Toggle</td>
      <td>On</td>
    </tr>
    <tr>
      <td>Spectator healing limit</td>
      <td>Minimum 0 times</td>
      <td>1 time</td>
    </tr>
    <tr>
      <td>Spectator healing cooldown</td>
      <td>Minimum 0 seconds</td>
      <td>0 seconds</td>
    </tr>
    <tr>
      <td>Starting health</td>
      <td>Minimum 1 HP</td>
      <td>100 HP</td>
    </tr>
    <tr>
      <td>Stage allowlist and blocklist</td>
      <td>List of stages</td>
      <td>All approved stages on allowlist; all pending stages on blocklist (only stage owners and moderators can remove from blocklist)</td>
    </tr>
    <tr>
      <td>Team selection method</td>
      <td>Selector: No teams, random, prioritize friends, or deprioritize friends</td>
      <td>No teams</td>
    </tr>
  </tbody>
</table> -->

<!-- ## Spectating
A player may spectate a round in their own server, or across public servers. Spectators will have the option to “cheer” for a player, giving them a +5 HP boost. This will have no effect on a player’s health if they already have 100% of their health.

Players will have the option to prevent spectators from outside of their own server. Players will not have the option to block same-server spectators because they can visibly see the player in the arena anyway. -->

<!-- 
## Activity recording
Contestant and game mode activity should be recorded and stored for review after the round ends. The following attributes should be recorded:
* Contestant character position and orientation changes 
* Contestant health and stamina assignments changes 
* Contestant effect changes
* Contestant archetype ID changes
* Player connects and disconnects
* Bot personality assignments and changes
* Action usages 
* Item usages
-->


# Building in the Stage Maker
## Parts
Stage creators can add and delete parts in their stage.

### Modifiable part properties
The following part properties are modifiable:
* Color
* CastShadow
* Material
* Reflectance
* Transparency (max: 0.8)
* Size
* CFrame (Position, Orientation)
* Shape
* BackSurface
* BottomSurface
* FrontSurface
* LeftSurface
* RightSurface
* TopSurface

### Modifiable part attributes
Stage creators can change the durability levels of their parts, which defines how much damage the part can take before getting [destroyed](/standards/game-modes/turf-war/mechanics/destroyed-parts.md). 

<!-- ### Smooth modeling
The player can union, negate, intersect, and separate parts.  -->

## Action history
The player can undo and redo recent actions. When the player undoes something and does a new action, the redo history will be deleted.

## Zones
<table>
  <thead>
    <tr>
      <th align="left">Zone name</th>
      <th align="left">Zone description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Action zone</td>
      <td>Players can access this zone normally.</td>
    </tr>
    <tr>
      <td>Visible zone</td>
      <td>Players can see this zone, but they can't access it normally. The stage creator can make the arena stands invisible to players to give them more creativity over the layout.</td>
    </tr>
    <tr>
      <td>Invisible zone</td>
      <td>Players cannot see or access this zone.</td>
    </tr>
  </tbody>
</table>

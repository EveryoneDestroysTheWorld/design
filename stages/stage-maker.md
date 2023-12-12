# Stage Maker
When entering the Stage Maker, the player must be notified that they will give an irrevocable license to Beastslash that allows the company to use the stage for free. This will prevent players from sending DMCA takedown requests for their stages. 

## Building
Stage creators can build their stages with parts. The following part properties are modifiable:
* Color
* CastShadow
* Material
* Reflectance
* Transparency
* Size
* CFrame (Position, Orientation)
* Shape
* BackSurface
* BottomSurface
* FrontSurface
* LeftSurface
* RightSurface
* TopSurface

The player can also change the part's durability, which defines how much damage the part can take before getting "wrecked". 

### Smooth modeling
The player can union, negate, intersect, and separate parts. 

### Action history
The player can undo and redo recent actions. When the player undoes something and does a new action, the redo history will be deleted.

### Zones
<table>
  <thead>
    <tr>
      <th align="left">Zone name</th>
      <th align="left">Zone description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Action-safe zone</td>
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

## Navigation
The player can fly around the stage by pressing a specific button. The player can turn it off by pressing the same button. 

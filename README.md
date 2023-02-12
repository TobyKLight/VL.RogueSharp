# VL.RogueSharp
A vvvv gamma wrapper for the open source RogueSharp library by Faron Bracy

Nuget https://www.nuget.org/packages/VL.RogueSharp/

-----------------------
## Origin
Original library and documentation https://github.com/FaronBracy/RogueSharp
Referencing this nuget version 5.0.0 pre2 https://www.nuget.org/packages/RogueSharp/5.0.0-pre2

RogueSharp is originally intended for game development of roguelikes.
It is not a full set of tools to make a game. For example RogueSharp provides the pathfinding but the user would have to create their own movement system using the provided path. 

-----------------------
## What can it do? 
RogueSharp has functions useful for reasoning about 2D grids where some cells are walkable or transparent. 
For example pathfinding and field of view. 
Also includes a dice rolling function. 

VL.RogueSharp comes with a quick and dirty ASCII preview of the maps using VL.Skia. This is for preview purposes only, it's expected most users would take the map data and plug it into their own prettier drawing system.

Pathfinding 

![PathFinding](https://user-images.githubusercontent.com/4467208/160279650-d17d9547-f492-4a94-b411-cde4496013b8.gif)

Field Of View

![FieldOfView](https://user-images.githubusercontent.com/4467208/160279651-b63cb7f4-a68d-4f96-8ff4-1676af9eed08.gif)

------------------------
# Install  

* Install VL.RogueSharp via nuget 
In VVVV Gamma open the top left 'grey square' menu > Manage nugets > Commandline

* type 'nuget install VL.RogueSharp -version 2.0.0-pre'

* Open the vvvv gamma help browser and search 'Roguesharp' for example patches 

------------------------
# Version history
v2.0.0-pre
* BREAKING CHANGE Removed int2 datatypes in all nodes and replaced with Vector2. 
* Deprecated SetCell (int2). 
* Deprecated GridCoordToGridIndex (Int2) and GridIndexToGridCoord (int2) 
* Added Vector (Vector2 Split Round) as util to quickly splint a vec2 to integer32s.  
* This is because int2 is a stride datatype. Adds a lot of extra references to a compiled app just for one little convenience datatype. 
* Changed node 'AllCellsEmptyWalkeable' to 'SetAllCells' with transparent and walkable as default. 
* Added option 'ClampInputToGridSize' on all nodes that take X Y input. With this off an out of bounds request will give an exception. It is on by default. 
* Improved helppatches 
* Added option on SetBorders for isWalkable and isTransparent
* Compatibility checked with vvvv gamma 2022.5.0-577


V1.0.3-pre
* Ensured compatibility with vvvv 2022.4.11-1312 (RC4)  


-------------------------
# LICENCE 
Released under MIT Licence 

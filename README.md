# VL.RogueSharp
A vvvv gamma wrapper for the open source RogueSharp library by Faron Bracy

Nuget https://www.nuget.org/packages/VL.RogueSharp/

-----------------------
//ORIGIN
Original library and documentation https://github.com/FaronBracy/RogueSharp
Referencing this nuget version 5.0.0 pre2 https://www.nuget.org/packages/RogueSharp/5.0.0-pre2

RogueSharp is originally intended for game development of roguelikes.
It is not a full set of tools to make a game. For example RogueSharp provides the pathfinding but the user would have to create their own movement system using the provided path. 

-----------------------
//APPLICATION
RogueSharp has functions useful for reasoning about 2D grids where some cells are walkable or transaprent. 
For example pathfinding and field of view. 
Also includes a dice rolling function. 

VL.RogueSharp comes with a quick and dirty ASCII preview of the maps using VL.Skia. This is for preview purposes only, it's expected most users would take the map data and plug it into their own prettier drawing system.

Pathfinding 

![PathFinding](https://user-images.githubusercontent.com/4467208/160279650-d17d9547-f492-4a94-b411-cde4496013b8.gif)

Field Of View

![FieldOfView](https://user-images.githubusercontent.com/4467208/160279651-b63cb7f4-a68d-4f96-8ff4-1676af9eed08.gif)

------------------------
//USAGE 

-Install VL.RogueSharp via nuget 
In VVVV Gamma open the top left 'grey square' menu > Manage nugets > Commandline
type 'nuget install VL.RogueSharp -Version 1.0.2-pre'

-Open the vvvv gamma help browser and search 'Roguesharp' for example patches 

-------------------------
//LICENCE 
Released under MIT Licence 

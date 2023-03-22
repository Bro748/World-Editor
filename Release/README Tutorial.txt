Visit this link for a demonstration of the World Editor in action
https://youtu.be/MgeEBM9EKS4
This video is outdated! But mostly everything functions similarly or the same.

You can continue reading for more detailed instructions

to start, 
either open an existing world file by navigating to the World_XX.txt file
or create a new world by inputting a new acronym

If you're opening a vanilla world file and want to see MSC changes,
open it from the following path: 
Rain World\RainWorld_Data\StreamingAssets\mergedmods\world\

The first time a world is loaded it may take a few minutes to generate the pngs
these are stored in the Rooms folder so that the next time you load the world it can be instant

you can add rooms to the world by using the 'Add Room' button (multi-select allowed)

the 'Add Room' button will also reload a room if it is already present.
If a room is loaded incorrectly, use this to load the correct room.

You can save the current world any time, but it will go in the Output folder for now
This may be buggy, so save often! 
And double-check all the world formatting before replacing anything


default file management hotkeys:

-Save="Control & S"
-Load="Control & O"
-New="Control & N"
-Add Room="Control & A"

Edit subregions by clicking on it in the Edit menu


There are bunches of visibility options! Check the view panel

Panning, zooming, hiding different elements, changing colors, ect.

Default hotkeys for all of that are here


-Map View="Control & E" (dev view\canon view)

-Map Colors="Control & R" (cycles between none\layers\subregions) 
(colors changeable in DisplayColors.txt)

-Slugcat 0-8 "Shift & <1-9>" (slugcat creature spawns)
-Layer 1="Control & 1" (map layer visibility)
-Layer 2="Control & 2" (ect)
-Layer 3="Control & 3" (ect)
-Entrances="Control & T" (toggle entrance visibility)
-Connections="Control & Y" (ect)
-Dens="Control & U" (ect)
-Creatures="Control & I" (ect)

//navigation (Pan is hardcoded to nothing, for now anyways)
-Pan=""
-Zoom In="+"
-Zoom Out="-"

Now how about editing?? Yes, this application can do that too!!!!1!

Behind the scenes, 'edit modes' are how everything decides what you're currently trying to edit

When you hold a button (or in a few other specific instances,)
You go into a certain edit mode
And then clicking with the mouse is used to edit the actual thing

Let's go over each of them one by one


-Draw Connections="Shift"
click on an entrance and drag to the entrance it should connect to
behavior is slightly different if the entrance is already connected

-Room Move="Control"
click on a room to drag it to a new location

-Room Delete="X"
click on a room to delete it

-Room Layer="C"
click on a room to cycle through which canon layer it's on

-Room Subregion="V"
click on a room to cycle through which subregion it's set to

-Room Tags="Z"
click on a room to bring up a panel where you can select which tags it has (eg, GATE, SHELTER, ect)

-Copy Room Canon Pos="N"
click on a room to copy the canon pos position into the dev position

-Copy Room Dev Pos="M"
click on a room to copy the dev pos position into the canon pos


-Room Attractiveness="A"
click on a room to cycle through the attraction value for the currently selected creatures
(only works if Room Attractiveness mode is set for the creature panel in the edit menu)

Creature Panel Mode="Control & T" (hotkey to toggle Creature Panel; relevant above and below)

While in Creature Adding mode, drag a creature from the Creature Panel onto a den for quick adding


-Creature Delete="P"
click on a creature to delete it (will delete an entire lineage)

-Creature Add Quant="O"
click on a creature to add quantity or lineage chance (hold click to use linear knob editing)

-Creature Sub Quant="I"
click on a creature to subtract quantity or lineage chance (hold click to use linear knob editing)

-Add Creature To Den="S"
requires Creature Adding mode
click on a den to select it,
then if a lineage is desired, click on a creature in the den to select it, or on a +
(to add the creature as not a lineage, don't click on a creature)
then select the creature in the Creature Panel

alternatively, a creature can be first selected in the Creature Panel, and then the den selected

-Creature Properties="W"
click on a creature to bring up the Creature Properties panel
(this is the only way to edit scug-dependent spawns and tags)

-Den Properties="Q"
click on a den to bring it up in the Den Properties Panel
(in case you prefer the panel for adding creatures)

Many meta things can be modified through the .txts in the Settings folder

-Controls.txt
sets all the inputs for the different modes

-Creatures.txt
this determines what creatures exist - edit this to add your favorite custom creatures

-\Creature Sprites\ (in the root folder)
add the black and white icon to this folder to display it in-game 
(\White folder is not necessary)

-DisplayColors.txt
sets colors for different color modes, like layers, subregions, attractions, ect.
edit this if you have more than the default number of subregions

-Slugcats.txt
Sets which slugcats are editable
This is only half-implemented, 
so not all features would be available to any slugcats added

-RenderColors.txt
Sets what colors to use for the output texture
Leave as default if you want it to work in-game,
but for map makers it may be useful to change the colors

SOME NOTES ABOUT DOWNPOUR FEATURES THAT AREN'T IMPLEMENTED
Rain World 1.9 adds a new 'conditional links' system
which allows different slugs to have different world connections.
The World Editor does not load this, so it may mess up any regions that use it.

1.9 also adds maps and properties specific to specific slugcats, 
which is also not supported currently.

If you're modifying a vanilla region, 
for proper compatibility you should use modification files.

https://rainworldmodding.miraheze.org/wiki/Downpour_Reference/Modification_Files

The World Editor does not generate modification files,
but they'd basically involve cropping the file to only the changed details.
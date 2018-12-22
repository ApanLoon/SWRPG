# SWRPG
Dream project of an updated Star Wars RPG based on Knights of the Old
Republic with influences from The Old Republic MMO.

# Concepts
## Outline
* Splash screen
* Start game menu
  * New game
  * Load game
  * Options
  * Exit
* New game
  * Intro
  * Birth
    * Name
    * Species
    * Gender
    * Physical attributes (morphs)
  * Early life
    * Home planet
    * Social status
    * Basic training
      * Basic mental attributes
      * Basic skill set
  * Faction
    * Selection
    * Different cut sequence depending on faction, typically arriving
      at a training facility for the selected faction
* Load game
* Main game
  * Planet 1..n
    * Arrival cut scene
    * Play area
      * Companion 1..n
        * Selection of x active companions from a pool of n
      * Speeder
        * A speeder can NOT be put in your pocket, getting off it will
          park it in-world. Leaving it will make it stay where you left
          it
        * Auto pilot that can re-trace the nav points back to the
          ship/speeder hangar
        * All speeders MUST accomodate all companions, regardles of
          species - companions climb on board visually
    * Departure scene
  * Ship 1..n
    * Boarding a ship does NOT automaically take off. You might just
      want to access cargo hold or re-group without actually leaving
    * Play area
## Systems
### Inventory
You can only carry a small number of small items with you constantly and
over-encumberancs completely nullifies your ability to fight. However, you
can use a small cloaking device to mask an area where you can temporarily
stash items and order your ship droid to collect the items using a hover
sled that comes with your star ship. The droid can only get to the stash
if the way from the ship to it does not require any special skills that
the droid and the hover sled can't negotiate.
* A mechanic where thieves could detect and slice your cloaking shield to
  steal the items you stash
* It is impossible to carry large items, however, a Force user might be able
  to move them short distances into a stash. Non, Force users would have to
  call the droid and help it load the item on the hover sled. 
      
## UI
* Generic Window
  * Title/drag bar
    * Hide/Show - Shrink/expand window content
  * Content with "widgets"
* Grid widget - A grid of slots
  * Grid slot
  * DragTarget - With list of acceeptable types
  * Draggable - With list of types
* ActionBar - Small window with no title bar and a GridWidget
  * Lockabble - if locked, drag and drop actions are not triggered
  * DragTargets allow only useable items (actions, special tools and
    consumables)
  * Left-clicking a drag target makes the player use the action/item
* InventoryWindow - Window with title bar and a GridWidget
  * Right-clicking makes the player use the item if it is usable

# Iron designer challenge 5: War Without Frontiers (page 39)

In games featuring the territorial acquisition dynamic, and especially in war-themed games,
territories are rarely acquired through a comical foot race.
They're usually acquired through the death, regardless of how abstracted, of another player's bits.
As a result of that death, the player gets the other player's territory.
Whoever has the territory wins the war.
Another common dynamic, "destroy the opposing side," is used for games that don't have territory.

For ths exercise, however, you'll be punishing yourself beyond those traditional borders.
Simulate and resolve a Civil War battle _without_ using territorial acquisition or
destruction of all units on the enemy side as the primary gameplay dynamic.

Split into teams of two to four players.
Each team should do its best to come up with a game that fits the above constraints.
For a greater challenge, have each team choose an additional mechanic or dynamic
that the other team is not allowed to use.

## Components Required

* Materials to create prototype

## Deliverable

* Board-game prototype or
* Card-game prototype or
* Tile-based-game prototype

## Suggested Process

1. **Determine a theme.** Which battle does your game simulate?
2. **Identify mechanics.** Without territorial acquisition, does it make sense to even have territory?
   It might, or it might not. Consider how a player can win a battle other than claiming territory.
   What is the goal, if not territory? What kinds of mechanics can players perform to achieve that goal?
3. **Identify the conflict between players.**
4. **Playtest.** Every time you add a mechanic to the game, test it.
5. **Create deliverable**

## Variants

Instead of the Civil War, choose a different conflict. World Wars I and II are obvious choices. You could also use other conflicts like corporate acquisition, feuding neighbors, or competing chain stores.

-----

## Messhall Mayhem

Okay, this is actually a 1-player game.

You're a bus-boy at a confederate mess-hall.
This war will be won or lost by the brave soldiers who risk their life to fight for whatever we're fighting for.
But how can those brave soldiers give it their all when they have no energy? They can't.
That's where we come in. We feed em a hot meal that reminds em of the missus back home that they're fighting for.
Gives em energy, helps them do their best.
But how can a soldier eat if there's nowhere to sit? They can't.
That's where you come in, player... go bus them tables so our boys can sit down for a spell and get some grub in em.

Task: x number of soldiers eat food. (presumably x increases each round)

The mess hall is laid out in a grid system. A cell in the grid may be occupied by a person, table, chair, or spill.
You must navigate the grid with "h", "j", "k", "l".
You are equipped with a rag, when next to a spill, you may use a free hand to wipe it up by pressing "w".
Once wiped up, your rag is dirty and must be cleaned before you can wipe a new mess.
You clean your rag at the wash station, typically against one of the walls, go there and press "w"
Messes need to be wiped because soldiers won't walk over them,
causing them to find a route to their seat that doesn't traverse the mess. This can create bottlenecks.
Soldiers won't walk over chairs either, so you need to push chairs in as you go by with "p".

When your hands are free, you can dart between soldiers to do things like clean up a mess,
get to an obstructing chair, etc. When your hands are not free, you must use the same path that the soldiers use.

When a soldier arrives at their seat, they eat for some amount of time, then get up and leave.
some have manners and push their chairs in, but some don't. Especailly when there's a battle underway outside,
they tend to gobble their food down, make a lot of messes, and not stop to push their chair in.
This is reserved for the later rounds.

When at a table space
You can go into and out of select mode with "s", and navigate the items to select with the same "h", "j", "k", "l" keys.
Once an item is selected, you can pick it up with your left hand using "d", right hand with "f".
If you press "d" or "f" while that hand is full, you will instead put that item down on whatever item is selected.
This allows you to stack cups, bowls, silverware, etc.
Each item has a stack limit. Cups mayb be stacked 6 deep, plates 8 deep, trays 6 deep. Silverware may be stacked 4 deep.
You may place silverware on other items, including the topmost item of a stack.
A cup can contain 10 silverware. A plate may contain 6 silverware.
A tray may contain 2 plates, or 4 bowls, or 8 cups, or 8 silverware. These may be stacked.
You may mix and match the tray contents, e.g. 1 plate, 2 bowls.

When you are finished stacking your tray, you pick it up by selecting with both hands empty and pressing either hand's pickup key.
You must then navigate back to the wash station and drop it off there.

You receive bonuses every time you get the mess hall entirely clean of spills, every time you clear a spot at a table,
every time you clear an entire table, and every time you return with dishes. Generally, bonuses are cumulative,
so getting a bonus early when it's easy will increase the value of later bonuses when it's more difficult and your
goals shift towards keeping up with the dinner demand.


### Other thoughts

* Music and SFX are off by default.
  * If user turns on music, it pops up a dialog telling them to go turn on their stereo.
  * If user turns off music, dialog to turn stereo off.
  * If sound effects are turned on, they are represented with little "sound bubbles" saying things like "clink" and "chomp"

# Challenge 2 -- It's Mine! (page 36)

For this challenge, you'll be exploring the dynamic of territorial acquisition. If you haven't noticed already, this dynamic is present in the great majority of board games made today.

As in the previous example, this game should allow two to four players.
The game must obviously have some kind of territory which would be acquired. You may select from one of two win conditions:

* The first player to get all the territory wins
* The first player with the most territory after X turns wins.

As the game's designer, it's up to you to figure out the theme, the necessary game bits and the mechanics.

## Components Required

* Materials to create prototype

## Deliverable

* Board-game prototype or
* Card-game prototype or
* Tile-based-game prototype

## Suggested Process

1. **Determine a theme, if you desire.** Precisely what are the players trying to conquer here? A swamp? A piece of the turf?
   Maybe it's a wild band of monkeys who are determined to take over the zoo at night. Remember that you don't need a theme,
   but having one often helps game designers new ot the process identify potential mechanics.
2. **Continue using the same process as in Challenge 1.**

-----

Brainstorming:

Mechanics:

* The board consists of locations with access points to other locations, controlled by players
* The number of ways you have to access the location somehow plays into your ability to control it
* It's valuable to get a location that has many connections, because it allows you to access many places at once
* While this makes it powerful (it can support many other locations), this also makes it vulnerable (it has a large surface area from which it can be attacked)
* Players decide whether they want to attack or defend an adjacent tile, or defend their tile
* All players choose at once during the decision phase, but their decisions are kept secret (they can only see the board and what they are intending to do)
* After the decision phase is the resolution phase,
  * General Attack: units in conflict cancel each other out. A location does not need units on it to be controlled.
    * Cells: A(p1, s1) <-> B(p2, s1), A is controlled by player 1, with a strength of 1, and B is controlled by player 2 with a strength of 1.
      If A attacks B and B attacks A, then it looks like A(p2, s1) <-> B(p1, s2) ie there was no conflict, because they each left their territory unprotected and took over the other's
    * Cells: A(p1, s1) <-> B(p2, s1), A defends, B attacks A. Their forces are matched, they obliterate each other, leaving A(p1, s0) <-> B(p2, s0)
    * Cells: A(p1, s0) <-> B(P2, s1), B attacks A, leaving A(p2, s1) <-> B(p2, s0)
    * Cells: A(p1, s1) <-> B(P2, s3), A defends, B attacks A with a strength of 2. The first unit dies killing A's unit, the second takes over A, the third stays on B, leaving A(p2, s1) <-> B(p2, s1)
    * Cells: A(p1, s3) <-> B(P2, s3), A(2) -> B(1), B(2) -> A(1), leaves A(p2, s1) <-> B(p1, s1) ie each attacked with 2, defended with 1, so lost defender and 1 attacker, losing their space and gaining their opponent's
    * Unmoved troops are implicitly defending
    * Retreating costs nothing: A(p1, s0) <-> B(p1, s1) <-> C(p2, s3). If we have B(1) -> A, and C(2) -> B, then we are left with A(p1, s1) <-> B(P2, s2) <-> C(p2, s1)
  * Direct supporting cells: Direct support is like being on that location, including helping in attacks, but must move into that location on their current location at the end of the turn.
    * A(p1, s1) <-> B(p1, s2)  <-> C(p2, s0), A supports B, giving A(1) -> B -> C(0), B(2) -> C(0), leaving A(p1, s0) <-> B(p1, s0) <-> C(p1, s3), thus A was able to move to C by joining the attack (2 moves)
    * A(p1, s1) <-> B(p1, s2)  <-> C(p2, s0), A defends B, giving A(1) -> B, B(2) -> C(0), leaving A(p1, s0) <-> B(p1, s1) <-> C(p1, s2)
    * If not joining an attack, only one move is possible: A(p1, s1) <-> B(p1, s0) <-> C(p1, s1) <-> D(p1, s0). A(1) -> B, C(1) -> D, leaving A(p1, s0) <-> B(p1, s1) <-> C(p1, s0), <-> D(P1, s1)
    * Troops may allocate their troops as they like. Thus if A(p1, s0) <-> B(p1, s2) <-> C(p1, s0), and p1 wishes to have A(p1, s1) <-> B(p1, s0) <-> C(p1, s1), They can do: B(1) -> A, and B(1) -> C
    * A direct supporting attack is interrupted if the location they are joining is attacked: A(p1, s1) <-> B(p1, s1) <-> C(p2, s1), and B(p1, s1) <-> D()
  * Indirect supporting cells: Stay on their own location
  * Attacking unowned locations

troops can only move one cell at a time.
portal cells (cells tied to another location)
one-directional cells
Other mechanics: certain territories correspond to amount of units you can add to the board, you can then place the units to strengthen weak locations, or ones you want to attack from,
gaining a territory is more valuable than retaining a territory (it pays to be offensive)
alliances - can hold in one area of the board while not holding in another -- shared ownership

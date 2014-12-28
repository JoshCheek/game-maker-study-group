# Ch2: Game Design Atoms (pages 25-40)

## The game state and game views

**Game State** -- Collection of all relevant information that may change during play.

**Game View** -- Portion of the game state that a player can see (e.g. in Holdem, you can see your hole cards, the pot, and the community cards)

**Game Space** -- ?? (maybe all possible values that state can take?


## Players, avatars, and game bits

**Players** -- the agents who set the rules in motion

**Avatar** -- represents the player in the game

**Game Bits** -- physical pieces of the game (tiles, tokens, cards, board, etc)

## Mechanics

**Game Mechanics** -- All the ways to change the game state.

Common classes of mechanics:

* **Setup** -- Rules for how the game begins.
* **Victory conditions** -- Rules for how the game is won.
* **Progression of play** -- Who goes first, turn-based or real-time? etc.
* **Player actions** -- "Verbs", what players can do, and what effect those actions have on the game state.
* **Definition of the game view** -- What information a player has access to, why, how it can change over time.

## Dynamics

Pattern of play caused by mechanics (better info in ch1 notes)

Interestingly, there are also metagame dynamics, or dynamics that take place outside
of the space of the game (e.g. player alliances and StarCraft clans).


## Goals

Victory conditions, missions, quests. Often provide rewards.


## Theme

What the game is about.

> _Bohnanza_ is a game about bean farming. _Super Mario Bros._ is a game about a plumber searching through the Mushroom Kingdom to save a princess.

-- page 32

Not all games have themes, e.g. Tetris.

> _Clue_ could just as easily be about finding a lost mitten or your soul mate with exactly the same mechanics.

-- page 32


## What comes first?

Anything.


## Putting it all together

A nice example of the atoms and their implications (page 33).

## Resources

* [I Have No Words, and I Must Design](http://costik.com/nowords.html)
* [Formal Abstract Deisgn Tools](http://www.gamasutra.com/view/feature/3357/formal_abstract_design_tools.php)

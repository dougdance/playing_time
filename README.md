# playing_time

Helps track how much playing time each person on a team gets

# User Stories

* As a Coach, I want to create a Team.
* As a Coach, I want add Players to a Team.
* As a Coach, I want to create a Game.
* As a Coach, I want to specify which Players are available to play in a Game.
* As a Coach, I want to start a Game.
* As a Coach, I want to specify which Players are playing in the Game.
* As a Coach, I want to pause a Game.
* As a Coach, I want to end a Game.
* As a Coach, I want to see how much playing time each Player has in a Game.
* As a Coach, I want to see a report of how much playing time each Player had in a Game.
* As a Coach, I want to see a report of how much playing time each Player had in many Games.

# Data Model Design

* Person
  * Id
  * Name (string)

* Team
  * Id
  * Name (string)
  * Coaches (list of Person)
  * Players (list of Person)

* Game
  * Id
  * Team
  * Date (datetime)
  * Expected Length (duration)
  * Available Players (list of Person)
  * Start (datetime)
  * End (datetime)
  * Elapsed Time (duration)
  * Playing Times

* Playing Time
  * Id
  * Game
  * Player (Person)
  * Playing Time (duration)

# All Done

I found several apps out there that already do this, and my motivation is gone.

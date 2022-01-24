# Quick start guide
1. [Core idea](#core-idea)
2. [Create new game](#create-new-game)
3. [Game UI](#game-ui)

## Core idea
Though a computer game can never be fully realistic, a certain degree of realism makes a game more immersive
and interesting.
From our current knowledge in physics, our universe is governed by Einstein's theory of relativity.
Particularly, to describe things happening within a scale of ~100 light years, 
we need special relativity.
Roughly speaking, special relativity tells us that
* Information travel is bounded by the speed of light
* Time dilation: relative to an observer, the clock of a moving object ticks slower

Having arbitrary faster-than-light technologies, which many other space games do, is forbidden by
special relativity.

In contrast, special relativity is the core mechanics in this turn-based game.
As a consequence, you will see a few unconventional concepts:
* typically, you observe the past state instead of the current state of other players
* whenever you want to interact with a player, including yourself, you send a command.
The command travels at the speed of light
* time-dependent mechanisms may not be calculated once per turn due to time dilation

Due to the restriction of the speed of information travel,
you cannot directly control your whole territory.
Instead, you have a set of direct subordinates, and you can
ask them to do things by sending commands.
Your direct subordinates are also players, they may have their
subordinates, and they have autonomy.
You might also be a subordinate of other player!
If you are a fan of grand strategy game, you can probably
figure out that this is inspired by the Crusader Kings.

We believe this unconventional game design can give you a
special feeling of immersion as if this is how our future
will actually look like, given that our current understanding
of physics is not too far off.

## Create new game

### Main menu
When you first enter the game, you will see the main menu.

![main menu](./images/main-menu.png)

To create a new game, click the "New Universe" button.

### Generate New Universe
![new universe](./images/new-universe.png)

The default settings will generate a universe and each player has one star initially. 
Here are the settings you should consider to tune:
* Total number of AI + human player: the initial number of player in the universe
* Universe name: use a new name for a new game to prevent overriding your other saved games
* Universe x dimension: the universe has 3 spatial dimension (x, y, z), this determines the maximum of x
* Universe y dimension: determine the maximum of y
* Universe z dimension: determine the maximum of z, it is recommended to set this to a small value since it is harder
to interpret the visualization of a universe with high z dimension in this game

The ideal size of the universe depends on the spec of your PC.
A reasonable suggestion is (x dimension = 10, y dimension = 10, z dimension = 3).

Next, you can click the "Generate" button, it may take a while to generate the universe.

### Server settings
![server settings](./images/server-settings.png)

The game creates a server even if it is single-player.
For a single-player game, you may tune:
* Human input wait time limit: the game waits that many seconds a turn for your input,
your can select 10000000000 seconds (at the top of the select box) if you want nearly infinite wait time.

Click "Apply settings" to continue.

### Register player settings
![register player settings](./images/register-player-settings.png)

To register yourself as a human player in the server:
1. Choose "Human only" in "Type of available players"
2. Click "Update"
3. A set of id of available players will appear in the "Pci your player id" select box,
you can just leave it as "1"
4. You don't have to change the password for a single-player game
5. Click "Register" to register you as the player
6. If everything goes well, you will see "Registered player id: 1", now you can click "Start" to start the universe

## Game UI
![hello universe](./images/hello-universe.png)

Click "Hello Universe!" to enter the main game UI.

![game ui region](./images/game-ui-regions.png)

The UI is separated into 4 region:
1. [Top bar](#top-bar)
2. [World map]()
3. [Player Information]()
4. [Command Information]()

### Top bar
Top bar is 

####
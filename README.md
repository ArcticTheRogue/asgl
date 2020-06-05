# What is `asgl`?

*`agsl`, also known as Arctic's Simple Game Library.*

ASGL is a script written in Bash made for managing games.

Instead of opening a GUI to manage your games, ASGL offers a more terminal-friendly approach. With ASGL, you may list; modify or run your games.

## Installation

Installation of `asgl` is very simple, all you need to do is move or copy it to your `$PATH`, for example: `/usr/local/bin`.

## How to use `asgl`

Executing ASGL opens an interactive prompt, in which you can type commands to run; list or modify your list of games.

### Adding games

To add a game type `a` and then follow the prompts.

First you will be asked to enter the name of the game, then the executable for the game. 
Finally, you will be asked if you are sure if you want to add the game.

Here is an example:

```sh
$ asgl
Type a command (h for help): # a
What is the name of the game?: # xonotic
Where is the exectable for xonotic?: # xonotic-glx
Would you like to save this game?: [y/n] # Y
Adding xonotic!
Game Added!
```


### Listing games 

To list the games you have added to `asgl`, type `l` in the ASGL prompt, as seen below:

```sh
$ asgl
Type a command (h for help): # l

csgo
okami
swarmlake
xonotic
```

### Playing games

To play a game, type `p` inside the ASGL prompt. This can be observed below.

```sh
$ asgl
Type a command (h for help): # p

What game would you like to play?: xonotic
```

### Removing games
If for whatever reason you wish to remove a game you can do so by typing `r`, then following the prompts.

Firstly, you will be asked for the name of the game, and then to confirm that you want to delete it.
If you confirm then the game will be deleted from `asgl`.

```sh
$ asgl
Type a command (h for help): # r

What game would you like to remove?: # xonotic
Would you like to remove xonotic? [Y/n] # y
```


### Getting help
If you ever need help with `asgl` you can type `h` and you will be given all the commands and their functions.

```sh
$ asgl
Type a command (h for help): # h

a/A -------- Add a game.
r/R -------- Remove a game.
p/P -------- Play a game.
l/L -------- List games.
h/H -------- List of commands.
q/Q -------- Exit.
```


## Future Plans

In the future, I plan to extend this command with an extended set of functions, such as:

- Add categories
- Improve the list command
- Port to another language
- ~~Add the ability to import `.desktop` files~~ (I decided being able to import Steam libraries was a better idea)
- Making it so games are listed with a number and you play them with this number
- Add the ability to import Steam libraries

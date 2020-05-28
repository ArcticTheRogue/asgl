# What is `asgl`?

`asgl` or Arctic's Simple Game Library is a script written in Bash made for managing games.  I felt that you shouldn't have to use GUIs whenever you wanted to simply open a game so I made `asgl`.  `asgl` allows you to simply add, list, and play your games from it.

# Installation
Installation of `asgl` is very simple, all you need to do is move or copy it to your `$PATH`, for example: `/usr/local/bin`.

## How to use `asgl`

### Adding games

To add a game type `a` and then follow the prompts.  First you will be asked to enter the name of the game, then the executable for the game, and finally you will be asked if you are sure if you want to add the game.  If you confirm your game will be added.

Here is an example:

```sh
$ a
What is the name of the game?: xonotic
Where is the exectable for xonotic?: xonotic-glx
Would you like to save this game?: [y/n] Y
Adding xonotic!
Game Added!
```


### Listing games 

To list your games simply type `l`, then you will get a list of the games you have added to `asgl`:

```sh
$ a
l

csgo
okami
swarmlake
xonotic
```

### Playing games

To play a game simple type `p` and then when `asgl` asks you tell it the game you would like to play.

```sh
$ a
p

What game would you like to play?: xonotic
```

### Removing games
If for whatever reason you wish to remove a game you can do so by typing `r`, and then following the prompts.  First you will be asked for the name of the game, and then to confirm that you want to delete it.  If you confirm then the game will be deleted from `asgl`.

```sh
$ a
r

What game would you like to remove?: xonotic
Would you like to remove xonotic? [Y/n]
```


### Getting help
If you ever need help with `asgl` you can type `h` and you will be given all the commands and their uses.

```sh
$ a
h

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

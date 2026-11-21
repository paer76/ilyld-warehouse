# I Love You, Let's Die - the GameShell Warehouse

The Clockwork GameShell edition of *I Love You, Let's Die*, by Antoine Evray (Paer): a first-person duel between two lovers,
on a television set that doesn't exist. This repository is a **GameShell Warehouse**: the GameShell installs the game
from it by itself.

## On the GameShell
1. Connect it to Wi-Fi (Settings > Wi-Fi).
2. Open **Warehouse > Add new warehouse...** and type: `github.com/paer76/ilyld-warehouse` (then Enter).
3. Open it: **Dead Sleep - Channel 13 > I Love You Lets Die**. A downloads it (about 52 MB); A again plays it.

No Warehouse in the menu? Update the launcher (Settings > Update), then reboot.

## By hand (any GameShell, no Warehouse)
The game is one self-contained folder - its own SDL3 and its assets in it, nothing to install: put it anywhere and run it.
```
wget https://raw.githubusercontent.com/paer76/ilyld-warehouse/master/DeadSleep/ILoveYouLetsDie/file/ILoveYouLetsDie.tar.gz
tar xzf ILoveYouLetsDie.tar.gz -C ~/games
"$HOME/games/I Love You Lets Die/I Love You Lets Die.sh"
```
For a launcher entry: `mkdir -p "$HOME/apps/Menu/21_Indie Games"` and
`ln -s "$HOME/games/I Love You Lets Die/I Love You Lets Die.sh" "$HOME/apps/Menu/21_Indie Games/I Love You Lets Die.sh"`, then reboot.

Saves are in `~/.local/share/DeadSleep/ILoveYouLetsDie`: a newer version, or the same one somewhere else, keeps them.

## Channel 13 Theme

A GameShell skin in the look of the show: Channel 13's late-night broadcast. In the Warehouse:
**Themes > Channel 13 Theme**. A downloads it; A again installs and selects it. To change it back:
Settings > Skins > Default.

## Launcher Native, by Paer

A native (C++) GameShell launcher by Paer: the same menus, games, settings and Warehouse as the
stock one, much faster and lighter, with smooth GPU scrolling and skins. In the Warehouse:
**Launchers > Launcher Native** - A downloads it, A again installs it and reboots into it. To go back:
**Utils > Switch Launcher** (in either launcher) toggles between the stock launcher and this one. If it
ever fails to start three times in a row, the GameShell goes back to the stock launcher by itself.

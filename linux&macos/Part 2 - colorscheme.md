# Color scheme

## Prerequisite

- Ensure your terminal support 256 colors
- Ensure your terminal support `gogh`
  - Alacritty
  - Cygwin
  - Foot
  - Gnome
  - Guake
  - iTerm
  - Kitty
  - Konsole
  - Mate
  - Mintty
  - Pantheon / Elementary
  - Tilix
  - XFCE4

## Install

- Use the non-interactive mode with following code(if you can't clone the repo, you can simply download the zip and unpack it.
- Go to the path with cd command

  For example, for you the unpacked file names `gogh` and in the folder `Downloads`, you can run command `cd ~/Downloads/gogh/installs&&./"replace this with the name of color scheme"`

  ```sh
  # clone the repo into "$HOME/src/gogh"
  mkdir -p "$HOME/src"
  cd "$HOME/src"
  git clone https://github.com/Gogh-Co/Gogh.git gogh
  cd gogh
  
  # necessary in the Gnome terminal on ubuntu
  export TERMINAL=gnome-terminal
  
  # necessary in the Alacritty terminal
  pip install -r requirements.txt
  export TERMINAL=alacritty
  
  # Enter theme installs dir
  cd installs
  
  # install themes
  ./atom.sh
  ./dracula.sh
  ```

Now the color scheme is successfully installed. View the change in your terminal now! (For my color scheme, I use `flat-remix`). For `iTerm2` user, see [misc](./Part 5 - misc.md) and change your color theme.

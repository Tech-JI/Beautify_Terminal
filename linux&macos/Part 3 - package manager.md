# Plugin manager

For this part, I will show you the demo with `antidote` and `omz`.

Though we know that `omz` is a very user-friendly frame, it might be too heavy and lead to low efficiency. Moreover, it is not a package manager actual. So I will my plugin manager `antodote` which is light weight, fast but powerful.

## Install

See the [repo](https://github.com/mattmc3/antidote) and [official web](https://getantidote.github.io/) to install the package manager. (I think it is fairly easy since the doc is clear)

## Config

- See `conf` directory, add `autoload -uz promptinit && promptinit` if you use plugin provide prompt like `p10k` or `pure`.
- Use command `vi ~/.zshrc` and add following line to your `.zshrc` (If you meet problem,  [see](https://stackoverflow.com/questions/11828270/how-do-i-exit-vim))

  ```bash

  # Set up antidote
  #linux
  source ${ZDOTDIR:-~}/.antidote/antidote.zsh
  #homebrew user
  source $(brew --prefix)/opt/antidote/share/antidote/antidote.zsh

  # load plugin
  antidote load ${ZDOTDIR:-$HOME}/.zsh_plugins.txt
  ```

- `source ~/.zshrc`

- If you use latest version `omz`, you can refer to the sample config to fix `compdef not found` problem.

- For recommended plugin, see sample config, `zsh-syntax-highlighting` and `zsh-autosuggestions` is a must. `z` is also strongly recommended to fulfill fast switching your path. `extract` is a unpack plugin. `vscode` and `vi-mode` is recommended to `vscode` user and `vim` user (if you are not a vim user, I still strongly recommend it).

A kind reminder, if you encounter problem like `clone failed`, you may need command `git config --global http.proxy '{http or https or socks5}://127.0.0.1:{port of proxy}'`

Or you can simply use `omz` [tsinghua source](https://mirrors.tuna.tsinghua.edu.cn/help/ohmyzsh.git/) and refer to official document about how to use `omz`

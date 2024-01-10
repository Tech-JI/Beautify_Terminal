# Changing Prompt

**Note 1: This tutorial is for Windows Powershell and bash.** See [prompt](https://ohmyposh.dev/docs/installation/prompt) for other shells.

**Note 2: All `notepad` can be replaced with `vim` if you are using vim. (strongly recommended by @mQzLjP and many talented JISU-Tech members)**

## Powershell

1. `notepad $PROFILE` (if error, run `New-Item -Path $PROFILE -Type File -Force`)
2. Add the following line in `$PROFILE`, then SAVE:

  ```powershell
  oh-my-posh init pwsh | Invoke-Expression
  ```

3. Run `. $PROFILE` to reload. (You can ignore the error message, it might mean you have already changed the prompt before.) For Windows 11, use the command `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine` if the system forbid to run script.

## bash

1. `notepad ~/.bashrc` (or `~./profile`, depends on your system)
2. Add a new line: `eval "$(oh-my-posh init bash)"` and SAVE
3. `exec bash` (or `. ~/.profile` if you are using `~/.profile`)

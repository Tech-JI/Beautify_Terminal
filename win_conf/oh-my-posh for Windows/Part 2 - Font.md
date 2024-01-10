# oh-my-posh Font

## Nerd Font

Nerd Fonts are necessary for oh-my-posh. You can download them from [Nerd Fonts](https://www.nerdfonts.com/), but you can also directly download them in oh-my-posh CLI (recommended). For other ways to install Nerd Fonts, see [Fonts](https://ohmyposh.dev/docs/installation/fonts).

### Install Nerd Fonts in oh-my-posh CLI

Open Powershell and run the following command:

```powershell
oh-my-posh font install
```

Then follow the instructions. The editor of this tutorial (@mQzLjP) uses `FiraCode`.

### Configuration

#### Windows Terminal

1. Enable `Use the new text renderer ("AtlasEngine")` option in Terminal settings, or in `settings.json`:

```json
{
    "profiles":
    {
        "defaults":
        {
            "useAtlasEngine": true
        }
    }
}
```

2. Configure the font in `settings.json`:

```json
{
    "profiles":
    {
        "defaults":
        {
            "font":
            {
                "face": "FiraCode Nerd Font Mono"
            }
        }
    }
}
```

**See [Windows Terminal Config Guide](../Windows%20Terminal%20Config%20Guide.md) for more options.**

#### VS Code

When using Visual Studio Code, you will need to configure the integrated Terminal to make use of the Nerd Font as well. This can be done by changing the `Integrated: Font Family` value in the Terminal settings (default shortcut: `CTRL + ,` and search for `Integrated: Font Family` or via `Users` -> `Features` -> `Terminal`).

If you are using the JSON based settings, you will need to update the `terminal.integrated.fontFamily` value. Example in case of FiraCode Nerd Font Mono:

```json
{
    "terminal.integrated.fontFamily": "FiraCode Nerd Font Mono"
}
```

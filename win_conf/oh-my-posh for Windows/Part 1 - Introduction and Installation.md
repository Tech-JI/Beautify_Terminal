# oh-my-posh for Windows

## What is oh-my-posh

[oh-my-posh](https://www.github.com/JanDeDobbeleer/oh-my-posh) is a theme engine for Powershell. It can make your powershell prompt more beautiful and efficient.

For Windows, it's the best choice to make your powershell prompt more beautiful, but for Linux and MacOS, there're some better choices. So, **this guide is only for Windows users**.

## Install oh-my-posh on Windows

See [oh-my-posh](https://ohmyposh.dev/) for more details.

### Install prerequisites

- Windows 10/11
- Powershell 5.1+

### Install Windows Terminal

Install [Windows Terminal](https://apps.microsoft.com/detail/9N0DX20HK701) or [Windows Terminal Preview](https://apps.microsoft.com/detail/9N8G5RFZ9XK3) from Microsoft Store.

See [Windows Terminal](https://docs.microsoft.com/en-us/windows/terminal/get-started) and [Windows Terminal Preview](https://docs.microsoft.com/en-us/windows/terminal/get-started-preview) for settings.

### Install oh-my-posh

Open Powershell and run one of the following commands:

#### Winget (relatively slow)

```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```

#### Scoop

```powershell
scoop install oh-my-posh
```

or

```powershell
scoop install https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/oh-my-posh.json
```

#### With no package managers (Why?)

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; Invoke-Expression ((New-Object System.Net.WebClient).DownloadString('https://ohmyposh.dev/install.ps1'))
```

Then restart Powershell.

**Note: You should config the terminal before you proceed.**

### Update oh-my-posh

```powershell
winget upgrade JanDeDobbeleer.OhMyPosh -s winget
```

or

```powershell
scoop update oh-my-posh
```

or

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; Invoke-Expression ((New-Object System.Net.WebClient).DownloadString('https://ohmyposh.dev/install.ps1'))
```

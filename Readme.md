# Windows Terminal

Configuration for my Windows Terminal


##
Copy Microsoft.PowerShell_profile.ps1 inside $Profile

`> code $Profile`


## Files

**Windows Terminal configuration** (settings.json)

**OhMyPosh configuration** (ohmyposh-config.json)

![OhMyPosh segments](./Assets/OhMyPosh_1.png)

- Root
  - Elevated shell (Administrator)
- Path
  - Current path
- Dotnet
  - Current Active .Net Sdk Version
- Envvar
  - Current value of ASPNETCORE_ENVIRONMENT
- Executiontime
  - Execution time of the previously executed command
- Git
  - Git information when in a git repository
- Exit
  - Last exit code or that the last command failed

_Other states of the configuration_:

![OhMyPosh segments](./Assets/OhMyPosh_2.png)

![OhMyPosh segments](./Assets/OhMyPosh_3.png)

![OhMyPosh segments](./Assets/OhMyPosh_4.png)


**Powershell profile** (Microsoft.PowerShell_profile.ps1)

- Init __oh-my-posh__ config
- Import module __posh-git__ for tab completion
- Import module __Terminal-Icons__
- Set parameter completion for ```dotnet```
- Set parameter completion for ```winget```
- Set parameter completion for ```gh```
- Set Key-bindings (via PSReadLine Module)
  - <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>b</kbd> > ```dotnet build```
  - <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>t</kbd> > ```dotnet test```




### Credits / Inspiration / Docs

Scott Hanselman
- [Scott Hanselman's Blog Post](https://www.hanselman.com/blog/my-ultimate-powershell-prompt-with-oh-my-posh-and-the-windows-terminal)
- [Scott Hanselman's Powershell Profile (Gist)](https://gist.github.com/shanselman/25f5550ad186189e0e68916c6d7f44c3)

OhMyPosh
- [https://ohmyposh.dev/docs/](https://ohmyposh.dev/docs/)

Fonts
- [https://www.nerdfonts.com/](https://www.nerdfonts.com/)

Powershell profile
- [https://docs.microsoft.com/en-us/dotnet/core/tools/enable-tab-autocomplete](https://docs.microsoft.com/en-us/dotnet/core/tools/enable-tab-autocomplete)
- [https://github.com/microsoft/winget-cli/blob/master/doc/Completion.md](https://github.com/microsoft/winget-cli/blob/master/doc/Completion.md)
- [https://dominikjeske.github.io/pimp-my-terminal/](https://dominikjeske.github.io/pimp-my-terminal/)

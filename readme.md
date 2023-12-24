# Clone
1. Clone this in the home directory `cd`
1. `git clone git@github.com:777uliahshafar/dotfiles-win.git .config`

# Common Installation 
1. C++ `vc_redist.x64.exe`
1. windows terminal (available)
1. powershell (available)
1. winget (available), scoop `iwr -useb get.scoop.sh | iex`, chocolatey
1. git `winget install -e --id Git.Git`
    - Set up git config --global (if necessary)
    - Connect github with ssh.
1. neovim `scoop install neovim`.

PS: available on windows 11
change the executing policy `Set-ExecutionPolicy RemoteSigned`

# Windows Terminal config
1. Change the font to Inconsolata Nerd Font Mono Medium 15pt [font download](https://www.nerdfonts.com/font-downloads)
1. Place your config (terminal.json) to windows terminal config (setting.json)
1. Setting windows terminal appearance (font, transparency) and default.
1. Enable `Use ... text rendering (Atlas engine)` on Rendering for inverted color cursor. 

# Powershell Installation
1. oh-my-posh `scoop install https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/oh-my-posh.json`
1. PSReadLine `Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck`
1. posh-git `Install-Module posh-git -Scope CurrentUser`
1. terminal-icons `Install-Module -Name Terminal-Icons -Repository PSGallery`
    - [link](https://gist.github.com/markwragg/6301bfcd56ce86c3de2bd7e2f09a8839)
1. z `install-Module -Name z -Force`
1. PSFzf `scoop install fzf  && Install-Module -Name PSFzf -Scope CurrentUser -Force`.


# Powershell Config
1. Check the availability powershell profile `Test-Path $PROFILE`, false means it is not exist
1. Create powershell profile `New-Item -Type file -Path $PROFILE -Force`.
1. Edit the profile `nvim  $PROFILE`. 
1. Symlink it to your own config. Type `. $env:USERPROFILE\.config\powershell\user_profile.ps1` inside the profile (optional)
1. Install nerdfont for icon supporting.
1. Set windows terminal to use nerdfont font and powershell as default shell. This can be edited in json file of windows terminal.









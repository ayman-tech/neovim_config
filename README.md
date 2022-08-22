
# Neovim config like VScode

Make your Neovim look like VScode.

Unleash the power of Neovim by using it in this configuration.



## Installation

Open Terminal and enter the following commands to check if dependencies are present.
```bash
sudo apt update
sudo apt install neovim nodejs npm curl
```

After the dependencies have been met, we will now clone the repository into its location.
```bash
cd ~/.config/nvim
git clone
```
This installs the init.vim, coc-settings.json and snips folder at `~/.config/nvim` location.


We are going to need a tool named vim-plug to make this work which is enabled by one of the commands below:

##### Unix, Linux
```bash
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
  https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```
##### Linux (Flatpak)
```bash
curl -fLo ~/.var/app/io.neovim.nvim/data/nvim/site/autoload/plug.vim --create-dirs \
  https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
##### Windows (Powershell)
```bash
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
  ni "$(@($env:XDG_DATA_HOME, $env:LOCALAPPDATA)[$null -eq $env:XDG_DATA_HOME])/nvim-data/site/autoload/plug.vim" -Force
```

Now we will install plugins by opening the init.vim file
```bash
nvim init.vim
```
Now press ESC and type `:PlugInstall` to auto detect and install required plugins.
Once it shows completed, exit it and you are now done installing it.

If some icons arent displayed correctly, please check if terminal font is a nerdfont.
If not, download any of the nerdfonts from the link:
https://github.com/ryanoasis/nerd-fonts#patched-fonts


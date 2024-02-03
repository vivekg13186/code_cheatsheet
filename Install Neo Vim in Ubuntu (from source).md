## Who not 'apt install' or use flatpack ?
	You don't get latest version of Neovim ,you may find issue install latest plugins.

## Step to install from source 

1. Install tool needed for compiling
```bash
sudo apt-get install git ninja-build gettext cmake unzip curl wget font-config ripgrep build-essential xclip
```
2. Clone repo from git hub, you also download the zip file from GitHub
``` bash
git clone https://github.com/neovim/neovim.git --depth 1
cd neovim
```
3. Build the source 
```bash
cd neovim
make CMAKE_BUILD_TYPE=RelWithDebInfo
```
4. Make .deb package so easy to uninstall later
```bash
cd build && cpack -G DEB && sudo dpkg -i nvim-linux64.deb
cd ../..
rm -fr neovim
```
5. Install font icon (recommend for NV chad).cd to new location to install nerd font 
```bash
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v3.1.1/JetBrainsMono.zip
unzip JetBrainsMono.zip -d ~/.fonts
ls ~/.fonts
fc-cache -fv
```
6. Install NV Chad config 
```bash
git clone https://github.com/NvChad/NvChad ~/.config/nvim --depth 1
```

## Issue :
### For not showing ,need to set terminal app font to Jet Brain Mono font
-  [Setup nerd fonts in teminal](https://blog.danskingdom.com/Update-your-terminal-prompt-and-font-in-Windows-Terminal-and-VS-Code-and-Visual-Studio/)


## References
 - [NeoVim installation wiki 1](https://github.com/neovim/neovim/blob/master/INSTALL.md).
 - [NeoVim installation wiki 2](https://github.com/neovim/neovim/blob/master/BUILD.md#build-prerequisites)
- [Nvchad installation](https://nvchad.com/docs/quickstart/install)
- [ripreg installation](https://github.com/BurntSushi/ripgrep?tab=readme-ov-file#installation)
- [Nerdfonts](https://www.nerdfonts.com/font-downloads)
- [Setup nerd fonts in teminal](https://blog.danskingdom.com/Update-your-terminal-prompt-and-font-in-Windows-Terminal-and-VS-Code-and-Visual-Studio/)

![cover](./images/cover.png)

# dotfiles

```bash
# HomeBrew Install
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

```bash
# Git Install
brew install git
```

```bash
# iTerm2 Install
brew install iterm2 --cask
```

```bash
# Oh My ZSH Install
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

[Download Caskaydia Cove Nerd Font](https://www.nerdfonts.com/font-downloads)

```bash
# Clone Powerlevel10k Theme
cd ~ && git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

```bash
# Setup dotfiles
git clone https://github.com/tiagomassashi/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.p10k.zsh ~/.p10k.zsh
```

## How to extract current installed files?

```bash
cd ~/.dotfiles && brew bundle dump --force && git add . && git commit -m "file(Brewfile): update file" && git push
```

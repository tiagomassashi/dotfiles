![cover](./images/cover.png)

# dotfiles

```bash
# Brew Install
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
# Setup dotfiles
git clone https://github.com/tiagomassashi/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.p10k.zsh ~/.p10k.zsh
```

My dotfiles
-----------

These are config files to set up a system the way I like it.

## Installation

```
git clone git://github.com/osegrums/dotfiles ~/.dotfiles
cd ~/.dotfiles
rake install
./osx
```

Install homebrew q

```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
brew update
brew upgrade
brew bundle ~/.dotfiles/Brewfile
brew cleanup
brew bundle ~/.dotfiles/Caskfile
```

Install rvm

```
curl -sSL https://get.rvm.io | bash
```

Start services:

```
brew services start mysql
brew services start postgres
brew services start redis
```

[Configure git](http://help.github.com/git-email-settings/)

```bash
git config --global user.name "your-name"
git config --global user.email "your-email"
```

[Setup MacVim](https://github.com/carlhuda/janus)

```bash
mkdir -p ~/.vim/janus/vim/colors/tomorrow/colors
curl https://raw.githubusercontent.com/chriskempson/tomorrow-theme/master/vim/colors/Tomorrow.vim \
  -o ~/.vim/janus/vim/colors/tomorrow/colors/Tomorrow.vim
```

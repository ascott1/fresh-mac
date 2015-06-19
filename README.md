# fresh-mac
> A guide to how I set up a new machine

OS X 10.10

## System Preferences

### Desktop and Screensaver

- Screensaver: Ken Burns, Cosmos

### Dock

- Position on screen: `left`
- Check: `Automatically hide and show the Dock`

### Notification Center

Remove all notifications from:
  - FaceTime
  - Game Center
  - Reminders

### Trackpad

### Spotlight

- Uncheck: `Bing web searches`

### Displays

- Uncheck: `Show mirroring options in the menu bar when available`


### Date & Time

`> Clock`

- Uncheck: `Show day of the week`

## Install Xcode

- Install Xcode from the App store
- Open Xcode and accept the terms and conditions
- Install Xcode command line tools:

```
xcode-select --install
```

## Finder configuration

Open Finder > Preferences

In the sidebar check to show the home folder and hide unneeded folders (All My Files, etc).

### Show the Library folder

1. Open your the home folder.
2. Choose View > Show View Options (or press Command-J).
3. Near the bottom of the resulting View-Options palette is a setting called Show Library Folder.


## Homebrew

Install Homebrew

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
echo 'export PATH="/usr/local/bin:$PATH"' >> ~/.bash_profile
brew doctor && brew update
```

## Git

git comes pre-installed on OS X (or maybe bundled with the XCode dev tools), but let's use the homebrew version so we can update it when necessary.

```bash
brew install git
git config --global user.name "YOUR NAME"
git config --global user.email "YOUR EMAIL ADDRESS"
```

### Generate ssh keys

- [follow GitHub's guide](https://help.github.com/articles/generating-ssh-keys/) to work with Github.

### Global .gitignore

```bash
git config --global core.excludesfile ~/.gitignore
```

Add:

```
.DS_Store
*.swp
```

## Node

### Install nvm

[nvm](https://github.com/creationix/nvm) is a version manager for node.

```
curl https://raw.githubusercontent.com/creationix/nvm/v0.25.0/install.sh | bash
```

### Install node & io.js

```bash
nvm install stable # installs the latest stable version of node
nvm install iojs
nvm alias default stable # set the stable version of node as the default in any new shell
```

### Setup npm publish

```bash
npm adduser
```

## Ruby

Install `rvm`, Ruby 2.2.2, and Jekyll

```
brew install rbenv ruby-build

# Add rbenv to bash so that it loads every time you open a terminal
echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
source ~/.bash_profile

# Install Ruby
rbenv install 2.2.2
rbenv global 2.2.2
ruby -v

# Install Jekyll

gem install jekyll
```

## iTerm2 & Dotfiles

- Download the [iTerm2 color schemes](http://iterm2colorschemes.com/)
- `./dotfiles` contains some sensible default settings, based on those [put together by my coworkers](https://github.com/cfpb/dotfiles)


## Code font

Download [Input](http://input.fontbureau.com/) and set InputMono as the default typeface in Atom and iTerm2.


## Applications to install

- [Chrome](http://www.google.com/chrome/)
- [1Password](https://agilebits.com/onepassword)
- [iTerm2](http://iterm2.com/)
- [Alfred](http://www.alfredapp.com/#download)
- [F.lux](https://justgetflux.com/)
- [Dropbox](https://www.dropbox.com)
- [Spectacle](http://spectacleapp.com/)
- [Atom](https://atom.io/)
- [Unarchiver](https://itunes.apple.com/us/app/the-unarchiver/id425424353?mt=12)
- [Rdio](http://www.rdio.com/home/en-us/#apps)
- [iA Writer](https://itunes.apple.com/us/app/ia-writer/id439623248?mt=12)
- [Day One](https://itunes.apple.com/us/app/day-one/id422304217?mt=12)

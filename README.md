# fresh-mac
> Guide for how I set up a new machine

OS X 10.10

## Step 1: System Preferences

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

## Step 2: Install Xcode

- Install Xcode from the App store
- Open Xcode and accept the terms and conditions
- Install Xcode command line tools:

```
xcode-select --install
```

## Finder configuration

## Homebrew

Install Homebrew

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
echo 'export PATH="/usr/local/bin:$PATH"' >> ~/.bash_profile
brew doctor && brew update
```

## Git

git comes pre-installed on OS X, but let's use the homebrew version so we can update it when necessary.

```
brew install git
```


## Node

- nvm

## Dotfiles

## Applications to install

- Chrome
- 1Password
- iTerm2
- Alfred
- F.lux
- Dropbox
- Spectacle
- Sublime Text
- Atom
- Unarchiver
- Rdio

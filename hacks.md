**Show directory path in the Finder title**

`defaults write com.apple.finder _FXShowPosixPathInTitle -bool YES; killall Finder`

To undo: 

`defaults write com.apple.finder _FXShowPosixPathInTitle -bool NO; killall Finder`


**Make hidden apps (⌘+H) more visible by making inactive app translucent**

`defaults write com.apple.Dock showhidden -bool TRUE; killall Dock`

To undo:

`defaults write com.apple.Dock showhidden -bool FALSE; killall Dock`

**Delete the animation between revealing a hidden dock**

`defaults write com.apple.dock autohide-time-modifier -int 0;killall Dock`

To undo:

`defaults delete com.apple.dock autohide-time-modifier;killall Dock`


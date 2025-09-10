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

**More than four commands for text context in the submenu.** 

`defaults write -g NSServicesMinimumItemCountForContextSubmenu -int 99`

To undo:

`defaults delete -g NSServicesMinimumItemCountForContextSubmenu`



**Quit Finder just like any other app.** 

`defaults write com.apple.finder QuitMenuItem -bool YES `

To undo:

`defaults write com.apple.finder QuitMenuItem -bool NO`


**Disable relative date.**

`defaults write com.apple.finder FXUseRelativeDates -bool false`

Undo:

`defaults write com.apple.finder FXUseRelativeDates -bool true`

**Set format for date columns for proper sorting.**

`defaults write NSGlobalDomain AppleICUDateFormatStrings -dict \
  1 "dd-MM-yyyy" \
  2 "dd-MM-yyyy" \
  3 "dd-MM-yyyy" \
  4 "dd-MM-yyyy"`

**Show directory path in the Finder title**

`defaults write com.apple.finder _FXShowPosixPathInTitle -bool YES; killall Finder`

To undo: 

`defaults write com.apple.finder _FXShowPosixPathInTitle -bool NO; killall Finder`


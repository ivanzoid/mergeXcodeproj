# mergeXcodeproj
This script will merge Xcode project in supplied directory with remote one in case of git merge conflict.

# Installation

1. `brew install ivanzoid/tap/merge-xcodeproj`

2. Add the following to ~/.gitconfig:
```
# Driver for merging Xcode project files
[mergetool "mergepbx"]
    cmd = mergepbx "$BASE" "$LOCAL" "$REMOTE" -o "$MERGED"
```

# Usage
After git conflict, run  
`$ mergeXcodeproj .`  
in folder which contains .xcodeproj.

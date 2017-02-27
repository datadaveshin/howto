#Switching versions:
From http://apple.stackexchange.com/questions/171530/how-do-i-downgrade-node-or-install-a-specific-previous-version-using-homebrew

Here's step by step.
```
To see your current node version

$ node --version
To see available node versions

$ brew search node
To unlink from current version

$ brew unlink node
Install any version e.g. 6

$ brew install node6-lts
To link installed version

$ brew link node6-lts
To see your current node version (again)

$ node --version
```

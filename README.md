# Launch Visual Studio Code From Terminal
A configuration to enable launching Visual Studio Code from terminal on Mac

## Motivation
Developers love terminal! Sometimes, however, we want to launch VS Code in a folder from terminal. Natively, VS Code does not provide this feature. We need to do some subtle configurations to make it work!

## Method
Add the following command to your bash initialization script. 

`export PATH="\$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"`

Reload your bash. Enter your favourite folder and try `code .` :)

## Reference
1. [Visual Studio Code on macOS](https://code.visualstudio.com/docs/setup/mac#_alternative-manual-instructions)

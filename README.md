# Launch Visual Studio Code From Terminal
A configuration to enable launching Visual Studio Code from terminal on Mac

## Motivation
Developers love terminal! Sometimes, however, we want to launch VS Code in a folder from terminal. Natively, VS Code does not provide this feature. We need to do some subtle configurations to make it work!

## Method
Add the following command to your shell initialization script (like `.bashrc` for bash, `.zshrc` for zsh). 

`export PATH="$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"`

Reload your shell (with `source ~/.bashrc` in bash or `exec zsh` in zsh). Done!

Now enter your favourite folder and try `code .` :)

Note:
1. A more subtle way to add customized intialization commands is to add a `.zsh` script to `~/.oh-my-zsh/custom/` folder with the command. The scripts that end with `.zsh` will be automatically executed on zsh initialization. In this way, we are isolating our custmized settings from the original setting of zsh, a more elegant solution!

## Reference
1. [Visual Studio Code on macOS](https://code.visualstudio.com/docs/setup/mac#_alternative-manual-instructions). Note that the [first solution](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line) of this post may not be persistent if you restarted your Mac. Personally I suggest the [alternative manual instructions](https://code.visualstudio.com/docs/setup/mac#_alternative-manual-instructions) in this post, which is also the method described in this README :)

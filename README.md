# ssh
Scriptable Multi SSH Client for Windows

## Features
The following Key-Featues make this ssh client specifically useful

- Powerful config system which supports
- relative includes and
- Recursive evaluation in order to
- support Host Groups
- Ability to define multiple Hosts at once

## Config Files

### User Config File

The User config Files is located at `%USERPROFILE%\.ssh\config`

###  System Config File

The ProgramData System Config File is located at `%ProgramData%\ssh\conf`

The etc System Config File is located in the `.\etc\config` File relative to the running `ssh.exe`

### Order of Application

The config File Order is like with git

**Commandline Arguments** overwrite **User Config** overwrites **etc System Config** overwrites **ProgramData System Config**

while

**ProgramData System Config** completes **etc System Config** completes **User Config** completes **Commandline Arguments**

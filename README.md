# SSHFS Manager
> A bash script for managing SSHFS connections.

#### Requirements
* bash
* sshfs

#### Note
The script has been created and tested on a Arch Linux (x86_64) machine with the following requirements versions:  
```
GNU bash, version 4.4.11(1)-release

SSHFS version 2.8
FUSE library version: 2.9.7
fusermount version: 2.9.7
using FUSE kernel interface version 7.19
```

#### Install
1. Download or clone this git repository on your machine.
2. Open ``sshfs-manager`` directory in terminal.
3. Run ``bash sshfs-manager.sh install`` and follow the install instructions on the screen.
4. Close current terminal and open a new one.
5. Run ``sshfs-mgr --help`` and enjoy!

#### Usage
Use ``sshfs-mgr`` in combination with a command from the list:  

| Command                               |  Description       
|---------------------------------------|:--------------
| ``install``                           | Start the process of script installation. User will be asked for the mount path under which all servers will be mounted.
| ``add-server``                        | Add new server form with required data: server address, SSH user, source & mount directories and SSHFS options.
| ``connect``                           | A list of added servers will be displayed and the user will have to choose a server to connect to.
| ``disconnect``                        | Disconnect all connected servers.
| ``disconnect [server]``               | Disconnect a specific connected server by providing the server address.
| ``help`` / ``--help``                 | Print help menu.

# armamm
ArmA 3 Linux Server Mod Manager for lgsm (Linux Game Server Manager)  
https://linuxgsm.com/  
https://github.com/GameServerManagers/LinuxGSM

*This is an independent project for lgsm and I am not associated with it.*

> Current Version: 0.7 alpha

## TL:DR

> downloads mods 
> manage .bikey Files
> update mods

### Features:

1. *Download Mods* 
> Uses the steamcmd which also downloads the server
> Downloads the mods into the steamcmd workshop directory
> Symlinks the mods inside the arma 3 servers mods directory
> How it works:
> You need to input the workshop id of the arma 3 mod
> The script then downloads each mod and symlinks the mod inside the server

2. *Manage .bikey Files*
> Requires you to have "verifySignatures = 2" enabled in your "arma3server.server.cfg, otherwise pointless  
> Adds the .bikey files to the arma 3 server keys directory
> And Removes them
> How it works:
> Adding Keys: searches all .bikeys in the workshop folder and asks the user if he wants to add the mod (+ displays the mods name)
> Removing Keys: mostly the same, but only searches them inside the server keys folder

3. *Update Mods*
> Consists of 2 methods 
> One is user driven, so he can only choose some, or all, depends on him  
> The other one is made to use it with cron
> So you can like start the script each day 5am and the script just checks each mod if there is an update avialable

#### Found Bugs or have improvements?

Please use the "Issues" (https://github.com/Deadalus3010/armamm/issues) section!

##### Thats all

Thanks for using the script!

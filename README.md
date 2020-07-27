# armamm
ArmA 3 Linux Server Mod Manager for lgsm (Linux Game Server Manager)  
https://linuxgsm.com/  
https://github.com/GameServerManagers/LinuxGSM

*This is an independent project for lgsm and I am not associated with it.*

> Current Version: 0.7 alpha  
> This script still has a few problems, when those are fixed, I will release the script  

## TL:DR
  
> Downloads mods   
> Manage .bikey Files  
> Update mods  

### Features:
  
1. *Download Mods*   
> Uses the steamcmd which also downloads the server  
> Downloads the mods into the steamcmd workshop directory, lowercases them afterwards  
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
  
4. *Count Mods*  
> Counts all downloaded Mods and .bikey Files  

5. *Lowercase*
> Lowercases all Mods inside the steam workshop directory  
  
#### Usage:  
  
> Download the armamm.sh file, open it and may edit the paths  
> The Script doesnt care which it is located  
> ** CURRENTLY ONLY WORKS FOR 1 SERVER, so you need one script for each Server **  
> Change the file permissions, so it can be executed  
> Then simply run *./armamm.sh*  
  
> To Download Mods:  
>> ./armamm.sh dl | ./armamm.sh download  
  
> To Manage .bikey Files:  
>> Add: ./armamm.sh ak | ./armamm.sh addkeys  
>> Remove: ./armamm.sh rk | ./armamm.sh removekeys  
  
> To Update Mods:  
>> Update manually: ./armamm.sh up | ./armamm.sh updatemods  
>> Cronupdate: ./armamm.sh cup | ./armamm.sh cronupdate  
  
> To Count Mods:  
>> ./armamm.sh co | ./armamm.sh count  
  
> To Lowercase Mods:  
>> ./armamm.sh lo | ./armamm.sh lowercase  
  
> Running the script without any or wrong parameters  
>> Shows the Help menu  

##### Found Bugs or have improvements?  
  
Please use the "Issues" (https://github.com/Deadalus3010/armamm/issues) section!  
  
###### Thats all  
  
Thanks for using the script!  

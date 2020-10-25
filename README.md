![logo](https://i.imgur.com/gDbunES.png)  
Fall Guys - Free Advanced Internal Cheat - 1.2_5 - 20.08.2020  
Cheat is out of date, using it can expose your account to a ban!  
[![Discord](https://img.shields.io/discord/748288505507217428.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/AEfuvwT)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/xtejk)
  
  
## Beginning:
- A good way to get to know the cheat and its files and all the stuff related to it is  
by checking the wiki entries for answers to the most important questions.  
[https://github.com/xTeJk/Fall_Guys_Internal/wiki](https://github.com/xTeJk/Fall_Guys_Internal/wiki)
  
## How to:
- Check the publication date of the latest public branch (https://steamdb.info/app/1097150/depots/)
  - If it's the same as the version the internal fits, then download latest version [here](https://github.com/xTeJk/Fall_Guys_Internal/releases)
  - If it's not the same, go to https://github.com/xTeJk/Fall_Guys_Internal#offsets and update the offsets
- Start game in any configuration
- Inject cheat with [Xenos](https://github.com/DarthTon/Xenos/releases/download/2.3.2/Xenos_2.3.2.7z) (Native Inject / Existing Process)
- Press `INSERT` to open cheat menu
- Don't close console window!

## 0xC0000135 error while injecting
- Navigate to: `C:\Windows\System32`  
- Download `Xinput1_4.dll` [here](https://www.dll-files.com/download/2f11c2213a4d60a347b53a50277cd131/xinput1_4.dll.html?c=dWlEd2JPTnp5TmRTc1VHdkdlclAxQT09)  
- Paste `Xinput1_4.dll` in: `C:\Windows\System32`  
- Restart Xenos and inject once again
(thanks _Skill_ <3)

## Compilation:
- VS 2019 / v142 / .dll library
  - [Properties -> Advanced] -> Use multi-byte character set
  - [Properties -> C/C++ -> Preprocessor -> Definitions] -> `_CRT_SECURE_NO_WARNINGS`
- Compile as `Release x64` version

## Offsets:
- Download: https://github.com/Perfare/Il2CppDumper
- Choose metadata file from game directory
- Select `GameAssembly.dll` from game directory to load game binaries and unity's references
- Export to json
- Replace `il2cpp.h` to new one inside cheat files directory
- Replace offsets in `offsets.h` with new one from `script.json`
- Recompile

## Keybinds:
If you want to change keybinds use:  
https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes  
find interesting key `VK_` or `0x` code and put inside `menu.cpp` at correct place, eg.:  
`(io.KeysDown[VK_F1] && !OldKeysDown[VK_F1])`  
replace to:  
`(io.KeysDown[0x31] && !OldKeysDown[0x31])`  
to make flying mode bootable by `1` instead of `F1`.  

## Safe Values:
The code implements the recommended "safe" values of individual functions,  
they can be edited in the `values.h` file, but it's not recommended,  
because exceeding the recommended value may result in blocking the account.

## Visuals Colors
To edit the color of the visuals, search for `0xFF` in `render.cpp`  
and change the code after that phrase to your own RGB code, eg.:  
`0xFF589C21` (Green)  
replace to:  
`0xFF7E3EDE` (Red)  

## Functions:
All functions are possible for any configuration  
  
  Menu Key: INSERT
  
- GENERAL:
  - HOME » Hide Corner Text
  - DELETE » Panic Key (instantly closes game)
  - END » Unhook Cheat (disable cheat, keep game alive)
  - Disable Safe Cheat Values
- VISUALS:
  - F5 » Real Doors (Door Rush)
  - F6 » Real Path (Tip Toe)
  - F7 » Non-Jinxed Players
  - F8 » All Platforms Visible (Fall Match / Fruits Match)
  - F9 » Player with Tail (Final)
- MOVEMENT:
  - F1 » Fly Mode:
    - Flying Speed
  - F2 » Speed Hack:
    - Movement Speed (Default: 9.5)
	- Movement Speed when Carrying Item (Default: 8)
	- Movement Speed when Grabbing (Default: 5)
  - F3 » Dive Boost:
    - Normal Dive Boost (Default: 16.5)
	- Air Dive Boost (Default: 7)
  - F4 » Gravitation:
    - Gravity Scale (Default: 1.5)
- COLLISIONS:
  - Disable Stuns/Knockdowns
  - Disable Object Collisions
  - Disable Player to Player Collisions
  - Disable Falling Down
- CARRYING GRABBABLE ITEMS:
  - F10 » Item Drop Force:
    - Normal Item Drop (Default: 50)
    - Dive Item Drop (Default: 90)
  - F11 » Equal Tussle Chances When Grabbed
- GRABS:
  - F12 » Super Grab Feature
  - Grab Detect Radius (Default: 6)
  - Grab Check Distance (Default: 2)
  - Grab Max Force (Default: 0.6)
  - Grab Break Time:
    - Normal Time (Default: 1.2)
    - Jump Time (Default: 0.01)
  - Arm Length (Default: 1)
  - Grab Check Prediction Base (Default: 0.1)
  - Grab Immediate Velocity Reduction (Default: 0.5)
  - Grab Cooldown (Default: 0.5)
  - Regrab Delay (Default: 2)
  - Release Regrab Cooldown (Default: 1)
  - Break Grab Angle (Default: 75)
  - Grab Separation Force (Default: 7)
  - Grabber Velocity (Default: 0.1)
  
![1](https://i.imgur.com/tPLjbK2.png)
![2](https://media.giphy.com/media/lMyPbfquGuXZtp4xo6/giphy.gif)
![3](https://media.giphy.com/media/MBfnnKtO0H7YFgITik/giphy.gif)
![4](https://media.giphy.com/media/WoR2PCgTLjCTAyA7tT/giphy.gif)
![5](https://media.giphy.com/media/hRyEd1yyebazh2YDjR/giphy.gif)
![6](https://i.imgur.com/Ge73we8.png)

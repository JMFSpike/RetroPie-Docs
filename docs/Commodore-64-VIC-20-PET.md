***
![c64](https://cloud.githubusercontent.com/assets/10035308/12191151/2f3aaf48-b58e-11e5-92e5-b39455579c63.png)
***
_The Commodore 64 is an 8 Bit personal computer introduced in 1982 by Commodore International. This model holds the world record for the highest-selling single computer model of all time._
***

| Emulator | Rom Folder | Extension | BIOS |  Controller Config |
| :---: | :---: | :---: | :---: | :---: |
| [VICE](http://vice-emu.sourceforge.net/) | c64 | .crt .d64 .g64 .t64 .tap .x64 .zip .prg | none | /opt/retropie/configs/c64/sdl-vicerc **and** /opt/retropie/configs/c64/sdl-joymap-c64.vjm|

## Emulator: [VICE](http://vice-emu.sourceforge.net/)

## ROMS
Accepted File Extensions: **.crt .d64 .g64 .t64 .tap .x64 .prg**

Place your ROMS in
```shell
/home/pi/RetroPie/roms/c64
```
## Controls
```shell
Start Game: Spacebar
Menu: F12
Select: Enter
Cancel: Backspace
Exit GUI: Escape

Changing Controls:
-Press F12 to enter menu
-Navigate to machine settings and press enter
-Navigate to Joystick settings and press enter
-Navigate to Joystick device in port 2 and press enter
-to use a numpad to play your game navigate to Numpad and press enter
     -Up: 8
     -Up/Right: 9
     -Up/Left: 7
     -Left: 4
     -Right: 8
     -Down: 2
     -Down/Left: 1
     -Down/Right: 3
     -Fire: 0
-to use a Joystick (gamepad) instead, navigate to Joystick and press enter
- to go back to the previous menu, use the left arrow key

SAVING CONFIGURATIONS:

Go into 
- settings management
- save settings on exit
- save current settings
- save hotkeys
- save joystick map

CUSTOM MAPPING
- Go back to Joystick settings by pressing backspace and navigate to Joystick 1 Mapping and press enter
- Press enter on each key followed by pressing the key on your gamepad you wish to be mapped.
- Press escape to exit the menu and return to your game
```
### Advanced Configuration
Once you've started and exited the VICE emulator at least once it will create a configuration file called `sdl-vicerc` in `/home/pi/.vice/` which is a symbolic link to 
```shell
/opt/retropie/configs/c64/ 
```
open the file "sdl-vicerc" and to double the screen size change
```shell 
VICIIDoubleSize=0
 
to VICIIDoubleSize=1 
```
## Troubleshooting
* There have been some reports of the emulator crashing when it exits requiring a hard reboot

## Other Commodore supported systems
In addition to Commodore 64, VICE emulator also emulates the following Commodore systems: 

- C128
- C64DTV
- almost all PET models
- PLUS4
- CBM-II (aka C610) 
- VIC20

which can be accessed through the [Runcommand Launch Menu](Runcommand).

![03062016_2322241](https://cloud.githubusercontent.com/assets/10035308/13558061/dc5eeade-e3b7-11e5-94cc-4891ccafe15a.png)

You can create dedicated systems (e.g. VIC20 ) in Emulation Station following these [instructions](https://retropie.org.uk/docs/Add-a-New-System-in-EmulationStation/).

Logos in SVG for Commodore Systems are [available](https://retropie.org.uk/forum/topic/3226/es-custom-svg-logo-pack-includes-specific-mame-logos).
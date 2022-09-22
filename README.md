![Main Board](https://i.imgur.com/sOlGxNL.jpg)

The FamicomBox+ mod has been designed to fix some of the design flaws in the Famicom Box design. The Famicom Box is designed to switch between 16 different cartridges, however in the original design some of the pins in the cartridge are common between the 16 cartridges such as IRQ, M2 and PPU /RD. This mod addresses the following issues:

* Demultiplexes M2 (Pin 38) to all 16 Cartridges
* Multiplexes /IRQ (Pin 15) from all 16 cartridges
* Multiplexes CIRAM /CE (Pin 57) from all 16 cartirdges
* Demultiplexes PPU A12 (pin 64) to all 16 Cartridges
* Demultiplexes PPU /RD (Pin 21) to all 16 Cartridges
* Supplies PPU /A13 (Pin 58) to all cartridges
* Isolates EXP0, EXP1, EXP2, EXP3, EXP4, EXP5, EXP7, EXP8 and EXP9 
* Allows 2 cartridges to utilise EXP6 for Expansion Audio with volume control. 
* Fixes an issue with open bus on games such as Paper Boy
* Disables the second RAM chip 6000 - 7FFF when in game, to allow SRAM and other functions. 
* Enables / Disables $5xxx when in game, this is used in some games and the Everdrive. 

### Famicom Box Warning

On a stock Famicom Box, the EXP Lines are connected to 5V or GND depending on which slot you use. This is used with the CIC to address each CIC individually. Some cartridges use these ports for debugging, Audio etc. If you have a stock Famicom Box you will damage certain cartridge if you plug them in.

### Limitations
This mod is rather complicated to install as there are many parts that you will need to modify to get it to work. You will need to have prior experience with de-soldering IC chips, soldering mod wires and debugging any issues that arise. 
This mod will not work with modern games that have tighter timings, as well as bootleg games bought from places such as AliExpress. 

### Tested Games
I have tested this with the following games:

* Castlevania 3 (Famicom with Expansion Audio)
* The Legend of Zelda
* The Adventure of Link
* Super Mario Bros
* Super Mario Bros 2
* Super Mario Bros 3
* Gauntlet II
* Tetris
* Snake Rattle N Roll
* The Little Mermaid
* Excitebike
* Tennis
* Duck Hunt
* Wrecking Crew
* Captain Planet and the Planeteers
* High Speed
* Yoshi 

I have also been able to use the Famicom Disk System, the RAM adapter will fit in Slot 14. The mod also works with an Everdrive. 

__There may be some games that will not work on this system. This could be down to timing issues. I cannot guarantee any game will work outside of the games tested.__

### Menu System 
The Menu system has been designed by Nintendo to check an internal database of games or for the Nintendo Header in the ROM. Most games do not have a correct header and will not be in the database, thus the game will be rejected. 
 
To get around this, we have modified the menu to still allow games to show up in the menu, however it will only display "NES GAME" instead of the actual game name. 

### 3D Prints
I have included some 3D prints that have used with the Famicom Box.  
 
The Modulator 3D print I used to replace the modulator with some custom connectors with my Famicom Box, I had fitted an NESRGB and this was where I mounted the video and audio connections. This is not required, but added incase you also want to RGB yours. 

The Replacement Coin box covers are the 2 covers on the right-hand side. If you remove the coinbox, you will need these to cover up the holes. 

The 72 Pin connector spacer is helpful if you use the Aliexpress connectors. See the installation guide for more details. 


### Special Thanks

I would like to thank Lidnariq for his time and knowledge to help me make this idea a reality, he was there to teach me what parts were different between the Famicom Box and what parts to include on my mod board. 

I would also like to extend a thank you to Fiskbit, who has helped with reverse engineering the Menu software and modifying it to allow other games to function. He has also improved the menu and fixed some bugs. 
The boot up of the console is now drastically improved due to changes made to the menu. 

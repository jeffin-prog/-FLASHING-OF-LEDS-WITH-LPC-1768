# FLASHING-OF-LEDS-WITH-LPC-1768

# AIM: 
   To interface and toggle the led with ARM LPC 1768 microprocessor           
           
# COMPONENTS REQUIRED:
##  HARDWARE:
ARM LPC1768
LED
## SOFTWARE:
KEIL MICRO VISION 4.0 IDE

# PROCEDURE:


⮚	Open the Keil software and select the New uvision project from Project Menu as shown below.
⮚	Browse to your project folder and provide the project name and click on save.
⮚	Once the project is saved a new pop up “Select Device for Target” opens, Select the controller (NXP: LPC1768) from NXP (founded by philips) and click on OK.
⮚	Select the controller (NXP: LPC1768) and click on OK.
⮚	As LPC1768 needs the startup code, click on Yes option to include the LPC17xx Startup file.
⮚	Create a new file by file → new to write the program.
⮚	Type the code.
⮚	After typing the code save the file as main.c eg. (abc.c).
⮚	Right click target and Add the suitable files to source group1 and header for the project.
⮚	Add the main.c along with system_LPC17xx.c.
⮚	Build the project and fix the compiler errors/warnings if any.
⮚	Code is compiled with no errors. The .bin file is still not generated.
⮚	Right Click on Target Options to select the option for generating .bin file.
⮚	Set IROM1 start address as 0x2000. Bootloader will be stored from 0x0000- 0x2000 so application should start from 0x2000
⮚	Write	the	command	to	generate	the .bin file	from
.axf file
Command: fromelf --bin projectname.axf --output filename.bin
⮚	in c/c++ → include paths → desktop (00-libfiles).
⮚	.Bin file is generated after a rebuild.
⮚	Check the project folder for the generated .Bin file.

# ADD FILES:
Target1:
Source group1:
Startuplpc17xx.s, main.c (t), delay.c (t), systemlpc17xx.c (t), gpio.c (t)
Header:
Delay.h, stdutils.h, gpioi.h

# PIN DIAGRAM :
 

# CIRCUIT DIAGRAM:
 
 
# PROGRAM:


 
# Output:








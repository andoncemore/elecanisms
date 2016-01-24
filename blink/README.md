Blink program
======

The steps to get the blink program up and running on the PIC24 are as follows:


1. Plug in PIC24 using a microusb into your computer. Put the PIC24 into bootloader mode by holding down SW1 while pressing the reset button. 
2. Next go into the **site_scons** folder in the elecanisms directory
3. Run the **bootoadergui.py** file using python from your command line. A gui should open on your computer which gives you some options. The gui should already be connected to the PIC24.
4. Back in your command line, navigate to the blink folder. When inside the folder, run SCONS to compile the blink.c file. Once you run SCONS, you should have a blink.hex file. 
4. Now go back to the bootloader gui. Click File > Import Hex. Import blink.hex, which is located in the blink folder. 
5. Back in the gui, click "Write", which should load the blink.hex file into the PIC24. Click "Disconnect/Run" to run the file. 

If you would like to edit the blink program, open the blink.c file. Make whatever changes you would like and then use SCONS in the blink folder to compile the blink.c file into the blink.hex file. 



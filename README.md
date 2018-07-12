# bb0.2
Inspired by Ben Eater's YouTube series on building an 8-bit breadboard computer, bb is a simulated computer in Logisim. These files can be used with Logisim to run programs on bb0.2 and modify the computer for yourself!

# Prerequisites
You must download Logisim available here: http://www.cburch.com/logisim/
Before running a program you must ensure that the ROM chips are loaded correctly. Open the bb0.2.circ file with Logisim, select Project -> View Simulation Tree in order to see the components laid out cleanly in the left hand area of the screen. Double-click on the CPU circuit, then right-click on the ROM chip and select Load Image. Navigate to the folder where bb's files live and select the bbAssembly0-2ROM file, then save bb in Logisim. Do the same for the DecimalDecoder circuit, except loading the bbDecimalDecoderROM. Once you have saved bb with the ROM chips loaded it will attempt to reload these circuits when it opens the circuit file, and you can safely reset or even close and reopen bb and the ROM chips will retain their contents.

# Tests
At the main circuit of bb reset the computer by pressing ctrl+r, then right-click on the HDD and select Load Image, then load the bbInfiniteAdd file and press ctrl+k to start the simulation. bb should now begin to add infinitely upwards by one, outputting the results of the computation onto the output display. Manipulate memory address 15 in the HDD in order to specify what integer to count by. You must reset and restart bb in order to reload the HDD with the new integer to count by. Logisim ROM and RAM circuits use hex.

# Authors
Austin Moss

# Acknowledgments 
Ben Eater - https://eater.net/

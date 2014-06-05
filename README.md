RPi-HY28b-adapter
=================

This is a simple Raspberry Pi shield for the HY28b 2.8" touch LCD. The LCD can then be used as the primary display by following the instructions here: http://www.instructables.com/id/HY28B-Touch-Display-with-Raspberry-Pi/ . To modify the layout you have to download this library: http://bioserver.her.hcmr.gr/RaspberryPi.html and put it somewhere in your Eagle library path. You may also have to put the file hy28b.lbr somewhere where Eagle can find it as a library.

The board is a two sided. But the layout is such that you can use the top layer for a one sided board and then wire the bottom side directly to the display pins. For that purpose there are sometimes two vias.

To make the make the assembled shield fit onto your Pi without colliding with the Ethernet jack you'll have to cut some unused pins from the display pcb and insulate them or the Ethernet jack with some tape.

On this board I also broke out the serial port to a matching pin configuration of my favorite USB to serial adapter (http://imall.iteadstudio.com/im120525005.html). I have not tried it yet but using it with the arduino IDE should be straight forward following these instructions: http://openmicros.org/index.php/articles/94-ciseco-product-documentation/raspberry-pi/288-programming-an-arduino-from-your-raspberry-pi-with-ciseco-hardware .

I also included the gcode I used to make the board on my CNC mill. The gcode was generated using pcb-gcode release 3.6.2.4 (download here: http://pcbgcode.org/list.php?12). It assumes a 0.1mm v shaped engraver going 0.05mm into the board. The outline is cut using a 1mm flute.

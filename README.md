## Adafruit USB Type C Power Delivery Dummy - I2C or Switchable - HUSB238 - STEMMA QT / Qwiic PCB

<a href="http://www.adafruit.com/products/5991"><img src="assets/5991.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit USB Type C Power Delivery Dummy - I2C or Switchable - HUSB238 - STEMMA QT / Qwiic. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5991

### Description

The HUSB238 USB PD sink chip is neat in that you can either use switches (really, resistor selection) to set the desired PD voltage or use I2C for dynamic querying and setting. We already stock a simple Adafruit USB Type C Power Delivery Dummy Breakout board around the HUSB238, but that one requires soldering closed jumpers to select the voltage. For folks who want a no-soldering-required board, this Adafruit USB Type C Power Delivery Dummy - I2C or Switchable is ready for instant gratification. No soldering required!

Compared to the basic Adafruit USB Type C Power Delivery Dummy Breakout we've done a renovation to keep the same great schematic and also add some oft-requested features:

* No soldering required! Switches allow on-the-fly voltage changes. Terminal block can be used to provide power to your robot, display, LEDs, etc.
* Green LED output lets you know that the terminal block power is on - can be disabled if you prefer
* Stemma QT for I2C control plug-and-play with Qwiic/QT
* USB Data lines available on solderable pads
* On/Off switch - you can disconnect the internal pass FET by connecting a switch between two onboard pads. When the switch is closed the output will disconnect / turn off.
* We use the HUSB328 PDL003A E-Marker variant of the chip, a little more expensive, but it can request 5A power.

It's perfect for USB Type C wall adapters providing multiple voltages. The standard offerings are 5V, 9V, 12V, 15V, 18V, and 20V. This HUSB238 breakout plugs into the USB C cable and negotiates the PD request and commands over the CC lines. For example, we can ask what voltages are available and pick the highest. Or if you need a specific voltage, it will select that one.

This breakout will be handy for projects where you need a lot more than 5V @ 2A power: this adapter can give up to 20V at 5A - yes you can get 100W over USB C! - and you could buck that down to get a ton of current at 5V or 12V if that's needed. Or use it to convert a DC or battery-powered device into a USB C powered one!

DIP switch-configured usage is simple: simply unplug the USB PD so you don't accidentally select too high a voltage for your device. Then switch ON the voltage you want: 5V, 9V, 12V, 15V, 18V, or 20V. You'll get that voltage and as much current as the adapter will provide. No microcontroller or microcomputer is required!

I2C-configured usage is also available via a Stemma QT port. Use the Arduino library and example code to query the USB Type C PD source for available voltages and currents and select the desired voltage dynamically. When configuring over I2C, the jumper settings are used on startup until the I2C commands come over.

The STEMMA QT connector lets you make solderless connections between your development board and the breakout or chain it with a wide range of other sensors and accessories using a compatible cable. QT Cable is not included, but we have a variety in the shop. 

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.

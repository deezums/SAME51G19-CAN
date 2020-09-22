# SAME51G19-CAN
Atmel ATSAME51G19A breakout board with TI TCAN33x transciever

![Index_photo](extras/photos/ATSAME51G19A_CAN_INDEX.jpg "Connection between MCP2515 and SAME51.")

This is version 1.0 of my ATSAME51G19A breakout board. 

Includes a 3.3V LDO, usb power, a led on PB22, reset switch, and 3V power led.

The canbus transiever contains a common mode choke, tvs array, and plenty of filter caps which can be optimally tuned to bus frequency. 

Digital split bus termiation using a mosfet array and resistors matched to rds, solder jumper allows disable, permanant pullup, or CPU control through PA21. 

Mostly 0402 components...

Tested working with atmel studio start examples and ATSAME54XPLAINED board. Hope to eventually port to Arduino with proper canbus library support.

Issues...

CMC pads should be narrowed vertically and can be horizontally compressed a fair bit.

Solder jumper pads are terrible, think too narrow and sharp. If not for 63/37 I don't think I could use them. 

TCAN33x, the extra function pins are not currently routed to CPU pins. Use TCAN332, or route the extra pins if you want to use hardware features of other variants.

Why did I make the silkscreen so small?! What pin is this!!

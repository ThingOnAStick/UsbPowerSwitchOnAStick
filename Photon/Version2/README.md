Usb Power Switch On A Stick
---------------------------

Control USB Power outlet to 2 USB A sockets via Photon.

Faults:
* V2.01
** ....
* V2.00
** 3v3 not connected to off board connector (D6/D6/GND/VBatt/RST/3v3).
** Excess top layer fill at Photon Keepout shown on PCB view (pdf issue only)


Changes:
* V2.00 - Added second USB A Socket. Removed current monitor, Added jumpers for TX/RX + 5V, A3-A5 + 5V, D6-D7 + 3v3 + RST and VBatt. New board size. Added gnd screen to USB A sockets.
* V2.01
** Fixed missing 3v3 trace for JP1. Improved silk screen. 
** Breaking: Moved control/flag D1-D4 -> D2-D5. Added JP4 to export D0/D1 for SDA/SCL or Switch 1+2 external. With 3v3 and 5V on connector.
** Moved JP1/2/3 to have 0.1" grid seperation between JP1 side and JP2/3. Moved JP4 to be on 0.1" grid with JP1/2/3 to allow for daughter board fitting on top with easy 0.1 grid.
** Beefed up vias for GND connection between USB Plug and PCB Bottom.
** Increased USB -> IC2 power trace to 0.05 (from 0.04)
** Moved Socket B -> R2 voltage monitor input via to be at top of board rather than crossing Photon Keepout area

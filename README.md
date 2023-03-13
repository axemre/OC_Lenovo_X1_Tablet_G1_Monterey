# OC_Lenovo_X1_Tablet_G1_Monterey
EFI config for running macOS Monterey on the Lenovo X1 Tablet G1 

This configuration is mostly working, but unfortunately, the trackpad on the X1 Thin Keyboard is not working. 

Specs:
* Intel Core m7-6y75 CPU (Skylake-Y) - Dual Core @ 3.1GHz max.
* 8GB LPDDR3-1866 RAM (soldered)
* 256GB SATA SSD (on my tablet)
* 12 inch 3K Display with touchscreen and stylus support
* LTE-A Module (Qualcomm X7)
* Intel DualBand Wireless AC 8265 combo with BT 4.2
* Mini-DisplayPort 
* 1x USB Type-C for charging and data transfer
* 1x USB-A 3.1

What works?

* Boot
* CPU power management 
* Thermal sensors
* Battery readings
* Cameras (back and front)
* Wi-Fi 
* Bluetooth 
* Audio (+ mic)**
* Touchscreen**
* Keyboard (external X1 Tablet keyboard)
* Everything else except the stuff listed

What does not work?

* Trackpad: This is a tablet and some models do not ship with the X1 Tablet Keyboard, and the implementation of the keyboard is pretty bad: The keyboard is connected using USB.. The trackpad is actually being detected by macOS, but it does not respond to any input. The TrackPoint (red small dot-like thingy in the middle of the keyboard) is working fine and the buttons for the TrackPoint also work just fine. I'm still trying to figure it out, but for now, it is sadly broken.
* Touchscreen: Although it is working, we should keep in mind that no Mac by Apple has native touchscreen support, and therefore, the touchscreen is not perfectly optimized like in Windows. Scrolling with the touchscreen is not working fine, other than that it is actually okay-ish. But in my opinion, the best solution is using an external mouse.  
* Audio: low volume from internal speakers. The speakers on that tablet are bad oob, so don't expect magical stuff to happen in terms of sound quality. It was bad, and it will be bad.
* Sleep (not tested, but I think that trackpad issues will surely prevent the device from going into sleep mode)
* maybe a lot more stuff is broken, but this is it for now. 

For any ideas and fixing broken stuff, feel free to open a issue to discuss about it. 


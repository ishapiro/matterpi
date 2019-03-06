This projects goal is to support the connection of 3d printers over a network connection with the MatterControl 3d printing application. 

https://github.com/MatterHackers/MatterControl

The basic approach is to create a Raspberry Pi Raspbian built that runs a Python script on startup.  This script will proxy any data
transmitted from MatterControl via Telnet to the connected 3d printer over a USB port.

The application relies on the "network support" built into MatterControl.  From what I can tell when this option is selected MatterControl
will initiate a telent connection, upon connect, to the IP address/Port specificed in the configuration panel.  Then all data MatterControl
would have transmitted to a serial port/USB will instead go over the TCP/IP Telnet pipe.

More to come ...

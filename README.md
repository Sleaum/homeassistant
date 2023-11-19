# homeassistant

owner
gervais T***

admin
Sleaum T***

users
savardiere savardiere



config/*.sh
config/configuration.yaml
config/www/planDeMasse.png


*****************************************
éviter d'utiliser /dev/ttyUSB*

For serial devices you should find them named by topology under /dev/serial/by-path/, so if you use the same usb hubs and ports it should stay constant. Eg:

ls -l /dev/serial/by-path/pci-0000:04:00.0-usb-0:2.1.1:1.0-port0
... /dev/serial/by-path/pci-0000:04:00.0-usb-0:2.1.1:1.0-port0 -> ../../ttyUSB0
Similarly, you should find the devices by name, sometimes including the serial number, under /dev/serial/by-id/, eg:

 ls -l /dev/serial/by-id/usb-FTDI_FT232R_USB_UART_A5771WOA-if00-port0
 ... /dev/serial/by-id/usb-FTDI_FT232R_USB_UART_A5771WOA-if00-port0 -> ../../ttyUSB0

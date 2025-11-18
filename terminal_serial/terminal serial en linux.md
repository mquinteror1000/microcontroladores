#terminal #serial
### averiguar nombre de dispositivo

```
sudo dmesg -l
```
Y conectar y desconectar el dispositivo para observar donde se montó
``` bash
[300990.406871] usb 1-5: new full-speed USB device number 20 using xhci_hcd
[300990.532406] usb 1-5: New USB device found, idVendor=1a86, idProduct=7523, bcdDevice= 2.54
[300990.532412] usb 1-5: New USB device strings: Mfr=0, Product=2, SerialNumber=0
[300990.532414] usb 1-5: Product: USB2.0-Ser!
[300990.533990] ch341 1-5:1.0: ch341-uart converter detected
[300990.534456] ch341-uart ttyUSB0: break control not supported, using simulated break
[300990.534780] usb 1-5: ch341-uart converter now attached to ttyUSB0
```
### Conectarse usando screen
```
sudo  screen /dev/ttyUSB0 38400

```
Resultado
```
temperatuea 
Comando no reconocido
temperatura
La temperatura es 1.95 C

```
### salir de screen
**Control + A, k, yes**

Siguiendo estas instrucciones logro conectarse un pic-pip 40 
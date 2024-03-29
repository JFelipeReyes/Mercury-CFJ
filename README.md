# CFJ Explorer
In this repository you can find all the relevant information for the development of this project, we have made use of the Python language to develop a client-server communication and through this execute the different functions that allow the movement of the device, and the native library of Linux motion to transmit what is captured by the camera through a port of the IP assigned to the Raspberry Pi.

## What's the use?

The idea behind the development of the project is to be able to explore narrow places no less than 17 cm high and 15 cm wide, since the device has a camera mounted on the chassis, which can be used to monitor the location of the device and possible obstacles it may encounter.

## How to use?

Steps to use the device :
**1)** Connect the Raspberry Pi to the power supply (Powerbank).
**2)** Connect the L298n diver to the Lipo battery.
**3)** Using the Linux terminal access the Raspberry Pi using SSH:

```
  $ ssh pi@ASSIGNED_IP.
```

**4)** Execute the Server.py file in the path it is stored:

```
  $ python3 Server.py
```

**5)** In the Linux terminal of the device that will act as a client, run the file Client.py:

```
  $ python3 Cliente.py
```

It is time to control the device:
The Client.py file runs a keylogger that detects the characters entered and sends a message that the Server.py file decodes and executes as a function.

**W** - This letter sends the command to advance to 25% power.

**S** - This letter sends the backward command at 25% power.

**A** - This letter sends the command to turn left at 40% power.

**S** - This letter sends the command to turn right at 40% power.

**Q** - This letter sends the command to stop.

**Y** - This letter sends the command to go forward at 100% power.

**H** - This letter sends the command to reverse at 100% power.

**K** - This letter disables the Server.

The power of the device is limited because in the transmission of the camera there is a delay of at least 0.5 seconds, therefore, by giving full power to the motors it is not possible to know with certainty the position of the device.

## How to install it?

* To install Rasbian we must use Raspberry Pi Imager which can be found at the following link:

* [Raspberry Pi Imager](https://www.raspberrypi.com/software/)

##  Information about Raspberry Pi 3 B+:

* [Raspberry Pi 3 B+](https://www.raspberrypi.com/products/raspberry-pi-3-model-b-plus/)

![Raspberry](https://github.com/JFelipeReyes/Mercury-CFJ/blob/master/Images/Raspberry.jpg)

* [GPIO](https://www.hwlibre.com/gpio-raspberry-pi/?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+hwlibreweb+%28Hardware+libre%29).

## Software

* [Motion](https://blog.osusnet.com/2009/03/13/televigilancia-con-motion-y-un-servidor-linux/).

* [Python](https://www.python.org/).

* [Apache2](https://httpd.apache.org/).

* [Atom](https://atom.io/)

## Pictures

* Schematic:
![Schematic circuit](https://github.com/JFelipeReyes/Mercury-CFJ/blob/master/Images/Esquematico.jpeg)

* Base:
![Base](https://github.com/JFelipeReyes/Mercury-CFJ/blob/master/Images/Soporte.jpeg)

* Device:
![Device](https://github.com/JFelipeReyes/Mercury-CFJ/blob/master/Images/Device.jpeg)

## Developers

* María Camila López López
* Juan Felipe Reyes Rubio
* Juan José Hernández Bravo

# VH-109 Radio

![VH-109 radio](https://store.ctr-electronics.com/cdn/shop/files/VH-109_WCP-1538_2048x2048_bfd9c84d-37a8-4bcf-9c32-a97cbfc1605c.webp?v=1729551120)

[VH-109 official documentation](https://frc-radio.vivid-hosting.net/)

The VH-109 is a radio, which is what allows the driver station(the computer) to connect to the robot without a huge wire running to each robot on the field. However, this also means that its wiring and setup is very important to get right.

 - Should be powered from the [RPM(Radio Power Module)](https://www.revrobotics.com/rev-11-1856/) for more simple, robust wiring
 - The radio power module's POE(power over ethernet) cable should run into the Ethernet port on the radio marked as "RIO"
 - If using coprocessors, or limelights then they should either be wired directly into the radio's other 2 Ethernet ports that are marked as "AUX1" and "AUX2", or if more ports are needed, into a ethernet switch that is connected to either of the aux ports
 - The radio should be exposed and easy to reach, as it will need to be taken out frequently enough, also, signal will degrade if it is not properly placed
 - The port marked as "DS" should be left open usually, as it is helpful for the programmers
 - The DIP switches on the back of the radio should be checked and flipped correctly before any of the Ethernet cables are connected OTHERWISE IT CAN AND WILL BREAK THINGS



|DIP Switch| Functions |
|--|--|
| Switch 1 | Controls POE of "AUX1" |
| Switch 2 | Controls POE of "AUX2" |
| Switch 3 | Activates the 2.4 GHz wifi access point (Should only be used outside of competition)|

# CANivore

![CANivore](https://robopiece.com/images/product/8d0191635154e10ee966bf1ac56bd33d.webp)

[Official Documentation](https://v6.docs.ctr-electronics.com/en/stable/docs/canivore/canivore-intro.html)

The CANivore is a device that allows for the creation of a secondary, completely separate CANbus. This CANbus, if properly utilized has several advantages over just expanding the RIO's inbuilt CANbus:

 - Simplifies wiring
 - Offers extra protection(Incase one CANbus breaks, some of your robot will still work)
 - Software features(such as timesync and better response times through CANFD)

However, there there is 1 major downside:

 - This will ___ONLY___ work with CTRE devices, any other devices will not work

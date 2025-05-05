# Power Distribution Hub

![PDH](https://cdn11.bigcommerce.com/s-t3eo8vwp22/images/stencil/1500x1500/products/602/3247/REV-11-1850-Power-Distribution-Hub-Top-FINAL__02549.1704386743.png?c=2&imbypass=on)

[Official REV Docs](https://docs.revrobotics.com/ion-control-system/pdh/overview)

The **Power Distribution Hub  or the PDH** is REV's power board for distributing power directly from battery.

The PDH is used for distributing power from the main 12V battery/120amp breaker to all the components on a robot, including motor controllers, VRMS, radios, RIOs and sensors.

## Features
    
-   **Output Channels**:
    
    -   1x Main Input with WAGO terminals
        
    -   20x 40A max outputs (8 high current, 12 low current)
        
    -   1x 20A protected channel (for VRM/PH)
        
    -   2x USB-C ports (diagnostics and firmware)
        
    -   1x CAN bus connection for telemetry and control
        
-   **Built-in Current Sensing** and **Voltage Monitoring**
    
-   **Status LEDs** for each channel
    

----------

## Wiring the PDH

### Wire Gauges

The connection from the battery should be wired with > than 6 AWG wire. 6 AWG is the BARE minimum and the standard for FRC wiring, lower gauges will require extra work.

### Input Wiring

-   Connect the PDH to the robot battery via the **120A Main Breaker** using 6 AWG wire.
    
-   Ensure positive and ground are securely clamped into the WAGO power input terminals.

### RIO Wiring

 - The RoboRIO should be connected directly to one of the small ports with a 5 amp breaker. **THIS IS THE ONLY LEGAL WAY TO WIRE A RIO** because it need regulated power.

## CAN Bus Integration

-   Connect the PDH to the robot CAN loop using the yellow/green twisted pair wires.
    
-   The PDH provides current and voltage telemetry to the roboRIO for monitoring and diagnostics.
    
-   Terminate the CAN loop properly at one end with a 120Ω resistor if required.
    
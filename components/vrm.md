# Voltage Regulator Module (VRM) - Electrical Documentation

![VRM](https://cdn.andymark.com/product_images/voltage-regulator-module/5bd3428561a10d292c9646c5/zoom.jpg?c=1540571781)

[Official Docs](https://ctre.download/files/user-manual/VRM%20User%27s%20Guide.pdf)

The **Voltage Regulator Module or the VRM** is a component that provides stable, regulated power to devices that require a consistent voltage, without fluctuations that can happen on the pdh's main power slots. This is important for smaller components like radios, sensors, and small controllers.

The VRM outputs  regulated 12V and 5V power at 500mAh and 2A.

## Key Features

-   **Input Voltage**: 5V-15V (just power off the PDH or PDP for 12V)
    
-   **Outputs**:
    
    -   2x 12V channels @ 2A each
        
    -   2x 5V channels @ 2A each
        
-   **LEDs** help you understand whether it is powering these slots
    

----------

## Wiring the VRM

### Wire Gauges

| Connection | Recommended Wire Gauge |
|--|--|
| VRM Input from PDH/PDP | 18 AWG (minimum), 16 AWG recommended |'
| 12V VRM Output | 18-22 AWG |
| 5V VRM Output | 18-22 AWG |


> **Tip**: Use ferrules or properly crimped connectors for a secure and safe connection.

### Input Wiring

-   Connect the VRM's input terminals to a 10A or 20A protected port on the Power Distribution Hub/Panel.
    
-   Ensure that positive (+) goes to the red terminal and negative (ground) (-) goes to black.
    

### Output Wiring

-   Wire regulated devices (such as the radio or vision processors) to the appropriate 12V or 5V outputs.
    
-   Double-check the voltage requirements for each device before connecting.
    

## Common Devices Powered by VRM

-   Robot Radio (12V output)
    
-   Raspberry Pi or Co-Processors (5V output)
    
-   Sensors and small custom circuits
    

> **Important**: The VRM is not intended to power large motors or any device drawing more than 2A per output.

----------

## Troubleshooting

|Symptom  | Possible Cause | Solution |
|--|--| -- | 
| LED off on a channel | No input power or overloaded output |Check input wiring and device current draw |
| VRM overheating | Overload or short circuit | Check the amperage provided or for breaks in power wires **in or out** |


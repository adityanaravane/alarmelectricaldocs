

[https://store.ctr-electronics.com/products/kraken-x60?srsltid=AfmBOoo7WWD-uK_QZSXQRtq9L8Cc4C7IS1b974rTVcNyUiOz1PFVmR3z](CTRE Docs)

The **Kraken X60** is a high-performance **brushless motor** developed by Cross The Road Electronics (CTRE) and Team REV Robotics. It’s designed to be the most powerful FRC-legal brushless motor to date, offering improved efficiency, torque, and durability compared to previous FRC motors such as the NEO or Falcon 500.

The Kraken integrates directly with **CTRE motor controllers** (like the Talon FX or new Phoenix 6 ecosystem) and includes **built-in sensors** for advanced control and telemetry.

---

## Features

- **Powerful Output**
    
    - Up to **600W of continuous power**
        
    - Peak torque around **4.7 N·m**
        
    - **Up to 6000 RPM** free speed (approximate)
        
- **Integrated Talon FX Controller**
    
    - Built-in motor controller reduces wiring complexity
        
    - Fully compatible with **CAN bus control via Phoenix 6**
        
- **Integrated Sensors**
    
    - **High-resolution encoder** for precise position and velocity control
        
    - **Temperature and current sensors** for safety and telemetry
        
- **Compact, Sealed Design**
    
    - Rugged aluminum casing
        
    - Sealed to reduce dust and debris ingress
        

---

## Wiring the Kraken X60

### Power Connections

- Connect power directly from the **Power Distribution Hub (PDH)** using **12 AWG wire** (minimum).
    
- Each motor should have its own dedicated breaker, typically **40A** for drive motors.
    
- Ensure all terminals are tight and fully inserted into the **WAGO** connectors on the PDH.
    

### CAN Connections

- The Kraken X60 communicates over **CAN bus**.
    
- Connect the **yellow (CAN High)** and **green (CAN Low)** twisted pair wires in series with the other CAN devices (PDH, RoboRIO, etc.).
    
- Maintain proper CAN bus topology and make sure one end of the bus is terminated with a **120Ω resistor**.
    

---

## Mounting and Cooling

- Use the **standard FRC motor bolt pattern** for secure mounting.
    
- The motor includes integrated cooling channels—avoid blocking airflow around the motor body.
    
- Optional **fan attachments** can improve performance under sustained loads.
    

---

## Programming & Control

- The Kraken X60 is compatible with **CTRE Phoenix 6 API**.
    
- Control modes include:
    
    - **Percent Output**
        
    - **Velocity Control**
        
    - **Position Control**
        
    - **Motion Magic**
        
- The integrated Talon FX reports telemetry like **current draw, velocity, temperature, and supply voltage** to the roboRIO.
    

---

## Best Practices

- Always **update firmware** using the **Phoenix Tuner X** application.
    
- Label each motor’s **CAN ID** clearly to avoid conflicts.
    
- Use **ferrules** and proper crimp tools for reliable CAN and power connections.
    
- Avoid long power wire runs to minimize voltage drop.
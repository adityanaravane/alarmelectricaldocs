[https://www.revrobotics.com/rev-21-1653/](Product Listing)

The **NEO 2.0** is REV Robotics’ second-generation **FRC brushless motor**, designed for high power density, precise control, and full compatibility with the **SPARK MAX** motor controller. It offers improved durability, better thermal management, and refined feedback sensing over the original NEO.

The NEO 2.0 remains one of the most efficient and reliable brushless motors for FRC, balancing **performance, control, and simplicity** for both drivetrain and mechanism applications.

---

## Features

- **Performance**
    
    - Up to **567W of continuous power**
        
    - **Free speed:** ~5676 RPM
        
    - **Stall torque:** ~3.36 N·m
        
    - **Peak current:** 105A
        
- **Integrated Hall Sensor**
    
    - Provides **position and velocity feedback**
        
    - Works seamlessly with the **SPARK MAX** controller for closed-loop control
        
- **Improved Construction**
    
    - **Enhanced bearings** and **thermal design** for higher load durability
        
    - **Updated encoder connector** for improved reliability
        
    - Fully **serviceable and reversible** design
        
- **Lightweight and Compact**
    
    - Weight: ~0.94 lbs (425 g)
        
    - Same footprint as a CIM motor for easy mounting
        

---

## Wiring the NEO 2.0

### Power Connections

- The NEO 2.0 connects to a **SPARK MAX** motor controller via **three-phase motor wires (A, B, C)**.
    
- Use **12 AWG wire** (minimum) from the **SPARK MAX** to the **Power Distribution Hub (PDH)**.
    
- Each motor should be powered through a **40A breaker** for drivetrain or **30A breaker** for mechanisms.
    
- Observe polarity when wiring power to the SPARK MAX (red = positive, black = ground).
    

### Sensor and Data Connections

- Connect the **6-pin encoder cable** from the NEO 2.0 to the matching port on the SPARK MAX.
    
- This enables **RPM, position, and temperature feedback** from the motor.
    
- Optionally, connect the **SPARK MAX Data Port** to the **roboRIO** via CAN or USB-C for configuration and telemetry.
    

---

## CAN Bus Integration

- Each **SPARK MAX** connects to the **robot’s CAN bus** via **yellow (CAN High)** and **green (CAN Low)** twisted pair wires.
    
- Maintain proper daisy-chain order between devices (PDH, SPARK MAXes, Pneumatic Hub, etc.).
    
- End the CAN loop with a **120Ω termination resistor** if needed.
    
- Use **REV Hardware Client** or **Phoenix Tuner X** (if mixed system) to manage device IDs and firmware.
    

---

## Mounting and Cooling

- The NEO 2.0 uses the **standard FRC CIM bolt pattern**, making it a drop-in replacement for CIM motors.
    
- Avoid blocking the **rear cooling vents**.
    
- REV offers compatible **planetary and ultra-planetary gearboxes** for direct mounting.
    
- Ensure alignment between motor shaft and gearbox to prevent bearing wear.
    

---

## Programming & Control

- The NEO 2.0 is controlled through the **SPARK MAX API** or **REVLib** for Java, C++, or LabVIEW.
    
- Common control modes include:
    
    - **Percent Output (open-loop)**
        
    - **Velocity Control**
        
    - **Position Control**
        
    - **Smart Motion (PID + motion profiling)**
        
- Telemetry available includes **temperature, current, voltage, and velocity**.
    

---

## Best Practices

- Always **update SPARK MAX firmware** before competition.
    
- Label each **CAN ID** clearly for easier troubleshooting.
    
- Avoid sharp bends or stress on the **encoder cable**.
    
- Check **motor temperature** during long practice sessions; add fans if sustained torque is high.
    
- Use **REV Hardware Client** regularly to monitor performance metrics and update firmware.
    

---

# Electrical and Electronics
This directory contains a collection of circuits and components that constitute the electrical and electronics module of the ventilator.


## Components
List of components.

| Component/Part                    | Summary                                                                                           | Quantity | Cost (Ksh) | Total Cost |
|-----------------------------------|---------------------------------------------------------------------------------------------------|----------|------------|------------|
| Raspberry Pi 4b                   | 8GB RAM 32 GB SD Quad Core 64 bit Processor Gigabit Ethernet                                      | 1        | 13000      | 13000      |
| Raspberry Pi LCD - 7" Touchscreen | Screen Resolution 800 x 480 pixels @ 60fps 24-bit color 10 finger capacitive touch.               | 1        | 13000      | 13000      |
| DC Motor                          | 12V DC, 30 rpm, 5 to 7 A, 70Kgcm IG32 Heavy Duty Planetary geared motored                         | 1        | 9500       | 9500       |
| VNH5019 Dc-Motor Driver            | 5.5V to 24V, 12A current up to 30A peak, Current Detection: 0.14 V/A, Maximum PWM Frequency: 20KZ | 1        | 1000       | 1000       |
| Oxygen Sensor                     |                                                                                                   |          |            |            |
| Solenoid Valves                   |                                                                                                   |          |            |            |
| Flow Meter                        |                                                                                                   |          |            |            |
| Pressure Sensor                   |                                                                                                   |          |            |            |
|                                   |                                                                                                   |          |            |            |


### VNH5019 Dc-Motor Driver
#### Features
1. Wide operating voltage range: 5.5 – 24 V

2. High output current: up to 12 A continuous
(30 maximum) per motor
3. Motor outputs can be combined to deliver up to 24 A
continuous (60 A maximum) to a single motor (see
Section 7)
4. Inputs compatible with both 5V and 3.3V systems (logic
high threshold is 2.1 V)
5. PWM operation up to 20 kHz, which is ultrasonic and
allows for quieter motor operation
6. Current sense voltage output proportional to motor
current (approx. 140 mV/A)
7. Motor indicator LEDs show what the outputs are doing
even when no motor is connected
8. Can be used with an Arduino or Arduino clone (through
shield headers) or other microcontroller boards (through
0.1″ header along the left side)
9. When used as a shield, the motor power supply can
optionally be used to power the Arduino base as well.



#### Board Connections

![DUAL VHN5019](https://a.pololu-files.com/picture/0J3755.1200.png?b32b98db0247112e0d969c6fb98814da)

Dual VNH5019 motor driver shield connected to a microcontroller (gray connections are optional)
source: [Datasheet Image](https://a.pololu-files.com/picture/0J3755.1200.png?b32b98db0247112e0d969c6fb98814da))



#### Pinout

| Pin      | Default State | Description     |
| ---        |    ----  |          --- |
| VIN      |        | The connection point for the positive side of the 5.5 – 24 V motor power supply. Since the overvoltage protection can be as low as 24 V, we do not recommend using 24 V batteries for VIN.   |
| VDD   |         | The connection point for the positive side of the logic power supply (typically 2.5 – 5 V). The only function of this pin is to power the internal pull-ups on the enable lines, M1EN/DIAG and M2EN/DIAG.      |
| VOUT   |         | This pin gives you access to the motor power supply after the reverse-voltage protection MOSFET (see the board schematic). It can be used to supply reverse-protected power to other components in the system but it should not be used for high currents. This pin should only be used as an output.      |
| GND   |         | Ground connection points for logic and motor power supplies      |
| MxA/B   |         | Output of half-bridge A/B. Each half-bridge connects to one terminal of a DC motor.     |
| MxPWM   | LOW        | Pulse-width modulation input: a PWM signal on this pin corresponds to a PWM output on the corresponding driver’s motor outputs. When this pin is low, the motor outputs are high impedance. When it is high, the output state is determined by the states of the MxINA/B and MxEN/DIAG pins.      |
| MxINA   | FLOATING        | Motor direction input A (“clockwise” input).      |
| MxINB   | FLOATING        | Motor direction input B (“counterclockwise” input).      |
| MxCS   |         | Current sense output. The pin voltage is roughly 140 mV per amp of output current when the CS_DIS pin is low or disconnected. The current sense reading is more accurate at higher currents. (Note that while the CS voltage can potentially exceed 3.3 V at high currents, the current sense circuit should be safe for use with many 3.3V analog inputs. Most MCUs have integrated protection diodes that will clamp the input voltage to a safe value, and since the CS circuit has a 10 kΩ resistor in series with the output, only a few hundred microamps at most will flow through that diode.)      |
| MxEN/DIAG   | HIGH        | Combination enable input/diagnostic output. When the driver is functioning normally, this pin acts as an enable input, with a logical high enabling the motor outputs and a logical low disabling motor outputs. When a driver fault occurs, the IC drives this pin low and the motor outputs are disabled. Note that the VNH5019 actually has separate EN/DIAG pins for each half bridge (ENA/DIAGA and ENB/DIAGB), but these are tied together on the board by default to create a single enable input/diagnostic output for each driver.    |
| MxCS_DIS   | LOW        | Disables the current sense output, MxCS, when high. Can be left disconnected in most applications.      |




#### Source
[VNH5019 datasheet](https://www.pololu.com/file/0J504/vnh5019.pdf)



### 12V DC 30RPM 70KGCM IG32 Heavy Duty
![RHINO 12V 30RPM 70KGCM HEAVY DUTY DC PLANETARY GEARED MOTOR](https://store.nerokas.co.ke/image/cache/catalog/motors/12V%20DC%2030RPM%2070KGCM%20IG32%20Heavy%20Duty%20Planetary%20Geared%20Motor-500x500.jpg)

[RHINO 12V 30RPM 70KGCM HEAVY DUTY DC PLANETARY GEARED MOTOR](https://store.nerokas.co.ke/index.php?route=product/product&path=150&product_id=2286)

#### Features
1. 30 RPM 12V Rhino Heavy Duty Planetary Geared, DC geared motors with Metal & Planetary Gearbox and Metal Gears
18000 RPM base motor
2. 4 stage gearbox for optimum high torque operation, which has breaking torque of 100 kgcm. Not recommended to use beyond 75 kg cm for continuous use
3. Motor rated Torque is 70 kg cm for continuous use at maximum efficiency.
4. Stall torque of motor is higher than 200 kgcm, but not recommedned to exceed 75kgcm.
5. Shaft is D type with total lenght of 16 mm and D shape in 12 mm.
6. 6mm Diameter shaft with M3 thread hole for tight mounting.
7. Shaft can be coupled using CNC coupling 6 mm or using fixed coupling as per requirement
8. Back shaft length is 9 mm
9. Gearbox diameter is 32 mm.
10. Motor Diameter 28.5 mm
11. Length 81.5 mm without shaft 
12. 300 gm weight
13. Supply Voltage : 12 V DC
14. No-load current : 800 mA, Load current : upto 7.5 A(Max)

#### Source
[Rhino Motion Control Solutions](https://rhinomc.com/products/dc-geared-12v-motor-t-driver/rhino-12v-30rpm-70kgcm-heavy-duty-dc-planetary-geared-motor-with-driver-rmcs-2110/)


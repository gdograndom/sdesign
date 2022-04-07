# DU 2021-2022 National Fluid Power Vehicle Challenge Repository

Micro Processor:
Raspberry Pi 3B - Head Node

## Solenoid Truth Table:

|               | Solenoid 9  | Solenoid 11  | Solenoid 16  |
|     :---:     |     :-:     |     :-:      |     :-:      |
| Direct Drive  |     LOW     |     LOW      |     HIGH     |
| Direct Charge |     HIGH    |     LOW      |     LOW      |
| Boost Drive   |     HIGH    |     HIGH     |     HIGH     |
| Regen Braking |     HIGH    |     LOW      |     LOW      |

## Pinout:

![alt text](https://www.raspberrypi.com/documentation/computers/images/GPIO-Pinout-Diagram-2.png)

### Solenoids:

Solenoid 9 = pin 31

Solenoid 11 = pin 33

Solenoid 16 = pin 35

### Other Pins:

Pi powered by 12V battery through voltage divider to pins 2(+) and 39(-)

Pins 3, 4, 5, 6 used for touchscreen power and touch input

Pin 1 supplies 3.3V VCC to 3.3V relays

## Full Electrical Schematic for Control: 
(Some pins inaccurate, refer to the above)
![Alt text](fullElectrical.png?raw=true "Full Electical Schematic for Control")

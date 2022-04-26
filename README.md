# DU 2021-2022 National Fluid Power Vehicle Challenge Repository

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

### Solenoid Activating Signals:

Solenoid 9 = pin 31

Solenoid 11 = pin 33

Solenoid 16 = pin 37

### Other Pins:

Pi powered by 12V battery through voltage divider to 5.5V to pins 2(+) and 39(-)

Pins 4,6 used for touchscreen power

Pins 3,5 SDA and SCL for I2C bus from ADS1015

Pin 1 supplies 3.3V VCC to 3.3V relays and ADS1015

## Full Electrical Schematic for Control: 
(Some pins inaccurate, refer to the above)
![Alt text](fullElectrical.png?raw=true "Full Electical Schematic for Control")


## Transducer Amplifier Gain Table
![alt text](https://939506.smushcdn.com/2600043/wp-content/uploads/2022/03/Table-2.png?lossy=0&strip=1&webp=1)

The converted voltage reading ranges from -2048 to +2047 for ADS1015.

So with gain of 1, analog_voltage = adc_value*(4.096/2047)

## Transducer/ADC Schematic
![Alt text](transducerSchematic.png?raw=true "Full Electical Schematic for Control")



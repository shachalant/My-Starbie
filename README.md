# starbie

![image alt](https://github.com/shachalant/starbie/blob/8e5e8b727aa895d1bbaf4562a835187e3bed0b66/images/starbie_3d_model.png)

A pocket-sized virtual pet device that lives on your desk, monitors your environment, and reacts to your interactions!

## Why I made this
As part of Hack Club's week 1 project for Half Life, I decided to follow the beginner's guide and create my first PCB project! Starbie combines a microcontroller, an OLED display, motion sensing, and environment monitoring into a custom designed PCB.

## What it does
- **Virtual Pet Animations:** Displays animated pet states on a 0.96" OLED screen.
- **Environment Sensing:** Reads room temperature and humidity using a DHT11 to influence the pet.
- **Motion Responses:** Detects movement, tilts, and taps using an MPU6050.
- **User Input:** Features tactile switch controls to feed, play with, and care for the pet.

## Hardware
| Part | Purpose |
| :--- | :--- |
| Seeed Studio XIAO ESP32-C3 | Microcontroller with built-in BLE |
| 0.96" SSD1306 OLED (I2C) | Pet display screen |
| MPU6050 Breakout | Motion and orientation sensing |
| DHT11 Sensor | Temperature monitoring |
| MX Switches & Keycaps | User input |
| 10 kΩ Resistor | Pull-up resistor for DHT11 data line |

## Pinout
| XIAO Pin | Connected To |
| :--- | :--- |
| `D1` | DHT11 DATA |
| `D2` | GPIO2 (Button / Switch Input) |
| `D3` | GPIO3 (Button / Switch Input) |
| `D4` | I2C SCL (OLED & MPU6050 Clock) |
| `D5` | I2C SDA (OLED & MPU6050 Data) |

## About
Created as part of the Hack Club Half-Life PCB design challenge

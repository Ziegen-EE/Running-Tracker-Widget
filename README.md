# Running Tracker Widget  
*A compact Arduino-based wearable for tracking pace, distance, and run duration.*

---

## Overview
The **Running Tracker Widget** is a portable, battery-powered device designed to measure and display **running metrics** such as **pace**, **distance**, and **elapsed time**.  
Built around the **Arduino Pro Mini**, this system integrates GPS positioning, user controls, and a display interface to deliver accurate real-time tracking data in a lightweight form factor.  

This project highlights hands-on skills in **embedded systems**, **circuit design**, and **hardware integration**, forming a complete end-to-end electrical engineering prototype.

---

## System Features
- **Arduino Pro Mini Core** – Compact 5V microcontroller board for low-power applications  
- **Adafruit Ultimate GPS Module** – Provides accurate positional data (lat/lon, altitude, speed, and time)  
- **LCD Display with Adjustable Resistor** – Displays pace, distance, and time in real-time  
- **Pololu LV Power Switch** – Enables safe and efficient power management for battery use  
- **User Input Buttons** – Right-angle momentary push buttons for start/stop and mode navigation  
- **Passive Components** – Decoupling capacitors and precision resistors for signal stability and protection  
- **9V Battery Snap Connector** – Supports portable power input with quick connection  

---

## Bill of Materials (BOM)

You can view the full interactive BOM spreadsheet here:  
👉 [**Running Tracker BOM – Google Sheets**](https://docs.google.com/spreadsheets/d/1CWu7IO52Xdz1FhUTgCzN4FMrNsjh3O-xI5pumeO5So4/edit?usp=sharing)

| # | Component | Manufacturer | MPN | Qty | Description / Notes |
|---|-----------|--------------|------|-----|----------------------|
| 1 | Arduino Pro Mini Socket | SparkFun | DEV-11113 | 1 | 5V, 16MHz, core microcontroller board |
| 2 | Adafruit Ultimate GPS | Adafruit | 746 | 1 | High-accuracy GPS module with integrated antenna |
| 3 | Pololu LV Power Switch | Pololu | 2808 | 1 | Low-voltage switch for efficient battery control |
| 4 | LCD + Variable Resistor | Adafruit | 181 | 1 | Display and control interface |
| 5 | Right Angle Push Button | C&K | 611-KSS223GLFG | 3 | User input buttons |
| 6 | Capacitor 10µF | TAIYO YUDEN | MCASL21GBB7106KTNA01 | 1 | Power line stabilization |
| 7 | Capacitor 0.1µF | KYOCERA AVX | KAM21BR71H104JM | 1 | Signal filtering |
| 8 | Resistor 220Ω | Panasonic | ERJ-S06F2200V | 1 | Current limiting |
| 9 | Resistor 10kΩ | KOA Speer | SG73P2ARTTD103G | 3 | Voltage division and logic pull-ups |
| 10 | 9V Battery Snap | Bourns | LS-00033 | 1 | Power supply connector |

---

## Functional Overview
1. **GPS Data Acquisition:** The Adafruit GPS module provides NMEA data for time, position, and velocity.  
2. **Microcontroller Processing:** The Arduino Pro Mini calculates pace and distance based on GPS data.  
3. **User Interaction:** Push buttons allow start/stop control and data viewing.  
4. **Display Output:** The LCD module shows real-time run statistics.  
5. **Power Regulation:** The Pololu switch ensures stable and safe power control from a 9V source.

---

## Technical Specifications
- **Operating Voltage:** 5V  
- **Input Power:** 9V battery (via snap connector)  
- **Microcontroller:** ATmega328P (Arduino Pro Mini)  
- **Display Interface:** Parallel/Serial LCD  
- **Sensors:** GPS (Adafruit Ultimate GPS)  
- **User Inputs:** 3x push buttons  
- **Enclosure:** Compatible with 3D-printed housing or handheld casing  

---

## Development Tools
- **IDE:** Arduino IDE  
- **Language:** C/C++  
- **Libraries:** `Adafruit_GPS`, `LiquidCrystal`, `SoftwareSerial`  
- **Simulation / Schematic:** KiCad or EasyEDA  

---

## Future Enhancements
- Add accelerometer or IMU sensor for step-based distance correction  
- Integrate Bluetooth for mobile sync  
- Log data to microSD for long-term performance tracking  
- Optimize firmware for lower power consumption

---

### PCB Manufacturing
The PCB layout and Gerber files were created following **[3DayPCBs](https://3daypcbs.com)** standard manufacturing specifications.  
Key parameters include:
- 1.6 mm board thickness  
- 1 oz copper weight  
- 6 mil minimum trace/space  
- Standard FR-4 substrate  
- Through-hole and SMD mixed design  

Compatibility with other PCB manufacturers may require DRC rule adjustments.

---

## License
This project is licensed under the [MIT License](LICENSE).  
Feel free to use and modify with attribution.

**PCB Design Notice:**  
All PCB and Gerber files included in this repository are designed according to **[3DayPCBs](https://3daypcbs.com)** manufacturing specifications, including board thickness, copper weight, trace width, and drill tolerances.  
Users adapting the design for other manufacturers should verify compatibility and adjust design rules accordingly.

---

## Acknowledgments

This project makes use of the [Arduino KiCad Library](https://github.com/Alarm-Siren/arduino-kicad-library)  
by **Alarm-Siren**, distributed under the [MIT License](https://github.com/Alarm-Siren/arduino-kicad-library/blob/main/LICENSE).

The library was used for schematic and footprint references during PCB design.

---

## Sponsorship & Support

This project is proudly supported by the  
**[School District 38 CTE (Career & Technical Education) Program](https://www.lewispalmer.org/cte)**.  

Their sponsorship provided access to electronic components, fabrication tools, and resources essential for the development and testing of the Activity Tracker Widget.  
Special thanks to the instructors and staff who promote hands-on STEM and engineering education.

---

## Author
**[Ziegen Ludwig]**  
Electrical Engineering Student | Embedded Systems Developer  
🔧 *Focused on IoT, microcontroller design, and wearable electronics.*


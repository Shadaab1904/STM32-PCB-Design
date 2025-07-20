# STM32-PCB-Design
KiCad project:  STM32 PCB Design on STM32F103C8T6

# About
This repository contains the KiCad 9.0 schematic for a custom-designed STM32-based development board. The board is built around the **STM32F103C8T6** microcontroller and provides core functionalities such as USB power, external clocking, GPIO headers, voltage regulation, and indicator LEDs ideal for prototyping, embedded systems development.

It includes: 

STM32F103C8T6:  ARM Cortex-M3 microcontroller (Blue Pill)     
USB_B_Micro: USB Micro-B connector for programming/power    
AMS1117-3.3: Voltage regulator (3.3V output)                
Crystal: External crystal oscillator with GND pads     
FB: FerriteBead: Noise filter on power rail
LED: Status or debug indicator
Resistor: For LED and pull-up/down functions
Capacitor: Decoupling and oscillator loading
Conn_01x04_Pin: 4-pin GPIO header                            
MountingHoles: Mechanical support for enclosure/PCB mount   

## 📂 Project structure
- `My_STM32_Board.kicad_sch` – Schematic file
- `My_STM32_Board_pcb` – PCB layout file
- `My_STM32_Board_pro` – KiCad project file
- `gerber/` – Gerber and drill files for fabrication
- `bom.csv` – Bill of Materials

- ## ⚙️ Tools
- Designed with [KiCad](https://kicad.org/)

- ## Features
  
- **Input**: USB Micro-B (5V)
- **Regulation**: 5V to 3.3V via **AMS1117-3.3** LDO regulator
- **Noise Filtering**: Ferrite bead between 3.3V rail and microcontroller

  Clock Circuit:

- Onboard **Crystal_GND24** oscillator provides accurate timing
- Crystal is connected to STM32’s OSC_IN/OSC_OUT with matching capacitors

  I/O and Connectivity:

- **USB Connector** allows firmware upload and power
- **4-pin GPIO Header** for serial comms, I2C/SPI, or digital I/O
- **LED Indicator** for debug or power status
- 

- ## 📦 Fabrication
Use the files in the `gerber/` directory to order PCBs from manufacturers (e.g., JLCPCB etc.).


- ## 📄 License
MIT License – feel free to modify and use.

## 🙌 Contributions
Pull requests welcome! If you spot issues or have improvements, please open an issue or PR.



STM8S Digital Timer
This project is a digital timer based on the STM8S103K3T6C microcontroller, designed to control an external load such as a relay or DC motor with flexible and precise timing intervals.

Users can configure two independent durations:

The waiting time (delay before activation)

The ON time (duration the output stays active)

For example, the device can be set to activate every 4 hours for 5 minutes.
A three-position switch allows selecting a wide time range from 1 second up to 99 days.
The output is driven through a transistor, capable of controlling loads such as relays or small DC motors up to 200 mA at 3 V.

The design emphasizes very low cost and simplicity, making it suitable for automation, hobby, and educational applications.

🧠 Features

Dual time interval (delay + on-time)

Adjustable from 1 second to 99 days

Transistor output driver (up to 200 mA)

Simple 3-button user interface

7-segment numeric display

Compact and single-sided PCB

Designed with Altium Designer

Firmware written in Keil (C for STM8S)

Final software version: March 2024

⚙️ How It Works

The user sets two time values (wait and active durations).

The microcontroller counts down the delay period.

Once the waiting time ends, it turns the output ON for the configured duration.

The transistor output stage can drive a relay, LED, or small DC motor.

The 7-segment display shows current timing values, and buttons are used for configuration and mode selection.

📸 Photos
Description	Image
Front side (components, display, and controls)	

Back side (PCB traces and STM8S)	

The final version of the board and firmware (March 2024) was also showcased on Instagram.

🧩 Hardware Overview (Low-Cost Build)
Component	Description	Min. Unit Price (USD)
STM8S103K3T6C	8-bit MCU	$0.80
7-segment display	1-digit LED	$0.25
Push buttons	3 pcs	$0.10
NPN transistor (e.g., S8050 / 2N2222)	Output driver	$0.05
Resistors	Standard ¼ W	$0.03 (total)
Capacitors	Electrolytic + ceramic	$0.10 (total)
Power jack / connector	DC input	$0.10
PCB (single-sided, local fab or DIY)	FR4 board	$0.50

💰 Total estimated minimum cost: ≈ $1.90 USD per unit
(prices based on minimum local/Chinese retail components in small quantity, early 2024)

🛠 Design and Development

Hardware Design: Altium Designer

Firmware Environment: Keil uVision (C for STM8S)

Microcontroller: STM8S103K3T6C

Output Type: Transistor switch (supports relay or DC motor up to 200 mA)

PCB: Single-sided copper board, manually etched and soldered

Final Software Version: March 2024

⚠️ Original schematic, PCB, and firmware source files were lost.
This repository serves as documentation and showcase of the design.

💡 Applications

Periodic automation (lighting, irrigation, ventilation)

Interval-based power control

DIY or educational electronics

Low-cost embedded control systems

📁 Repository Structure
STM8S-Digital-Timer/
│
├── README.md
├── photo_2025-10-08_13-49-49.jpg
├── photo_2025-10-08_13-49-55.jpg

✍️ Notes

This STM8S-based timer demonstrates how powerful and affordable 8-bit MCUs can be when paired with thoughtful circuit design and efficient firmware.
Even without source files, this documentation represents a solid record of embedded hardware and firmware development — a complete project finalized in March 2024.

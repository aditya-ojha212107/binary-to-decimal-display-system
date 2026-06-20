# binary-to-decimal-display-system

A complete digital electronics hardware project demonstrating the design, implementation, and testing of a **4-bit Binary to Decimal Display System** using standard **TTL Logic ICs**.

The system accepts a 4-bit binary input (0000–1111) and displays its corresponding decimal value (0–15) on two common-anode 7-segment displays. The project was designed and implemented entirely using digital logic hardware without any programmable device.

Unlike software-based implementations, this project relies solely on TTL logic circuits, providing practical experience in digital hardware design, binary arithmetic, BCD conversion, and seven-segment display interfacing.

---

## Project Objectives

* Design a hardware-based Binary to Decimal Display System.
* Convert 4-bit binary numbers (0–15) into decimal representation.
* Implement Binary Coded Decimal (BCD) correction using TTL logic.
* Interface two common-anode 7-segment displays.
* Verify the circuit through practical breadboard implementation.
* Demonstrate both manual and automated operation.

---

## Project Features

* Pure TTL Logic implementation
* No Microcontroller
* No Arduino
* No FPGA or CPLD
* Breadboard implementation
* Manual binary input using switches
* Automatic binary counting using a synchronous counter
* Two 7-segment decimal display output
* Complete hardware verification
* Demonstration videos included

---

## Components Used

### Digital Logic ICs

* 74LS85 – 4-Bit Magnitude Comparator
* 74LS83 – 4-Bit Binary Full Adder
* 74LS47 (×2) – BCD to Seven Segment Decoder/Driver
* SN74LS163 – 4-Bit Synchronous Binary Counter (Automatic Mode)
* CD40106 – Hex Schmitt Trigger Inverter (Clock Generation)

### Other Components

* Two Common Anode Seven Segment Displays
* Breadboard
* Toggle Switches
* 330 Ω Current Limiting Resistors
* +5V Power Supply
* Jumper Wires

---

## Working Principle

The project is implemented in two stages.

### Part 1 – Manual Binary Input

A 4-bit binary number is entered manually using toggle switches.

The 74LS85 Magnitude Comparator continuously compares the input with decimal 9. When the input exceeds 9, the comparator enables the 74LS83 Binary Adder to perform the required BCD correction.

The corrected BCD outputs are decoded by two 74LS47 ICs to drive the common-anode 7-segment displays, producing decimal outputs from 0 to 15.

---

### Part 2 – Automatic Binary Counting

The manual input stage is extended using the SN74LS163 synchronous binary counter.

A clock generated using the CD40106 Schmitt Trigger automatically advances the binary count from 0000 to 1111.

The existing comparator, adder, and decoder circuitry converts each count into its corresponding decimal display, demonstrating continuous automatic operation.

---

## Digital Logic Flow

Binary Input

↓

74LS85 Magnitude Comparator

↓

74LS83 Binary Full Adder

↓

74LS47 Decoder Drivers

↓

Common Anode Seven Segment Displays

↓

Decimal Output (0–15)

---

## Repository Contents

| File                    | Description                                  |
| ----------------------- | -------------------------------------------- |
| Circuit Schematic       | Complete hardware circuit design             |
| Breadboard Images       | Hardware implementation photographs          |
| Manual Demonstration    | Working images using manual binary input     |
| Automatic Demonstration | Images showing automatic counting operation  |
| Project Videos          | Manual and automatic hardware demonstrations |
| README.md               | Project documentation                        |

---

## Hardware Verification

The complete circuit was assembled on a breadboard and tested using all possible 4-bit binary inputs (0000–1111).

Both manual operation and automatic counting were successfully verified.

The hardware demonstrated accurate decimal outputs for all input combinations.

---

## Project Images

### Circuit Schematic

*(Replace this text with the circuit schematic image.)*

---

### Breadboard Implementation

*(Replace this text with the hardware implementation image.)*

---

### Manual Demonstration

*(Replace this text with photographs of the manual operation.)*

---

### Automatic Counter Demonstration

*(Replace this text with photographs of the automatic counter.)*

---

## Demonstration Videos

### Part 1 – Manual Binary to Decimal Display

*(Paste your YouTube link here.)*

---

### Part 2 – Automatic Binary Counter Demonstration

*(Paste your YouTube link here.)*

---

## Key Learning Outcomes

This project provided practical experience in:

* TTL Digital Logic Design
* Binary to Decimal Conversion
* Binary Coded Decimal (BCD)
* Magnitude Comparison
* Binary Addition
* Seven Segment Display Interfacing
* Breadboard Circuit Construction
* Hardware Debugging and Testing
* Digital System Integration

The project follows the complete engineering workflow:

**Digital Logic Design → Circuit Implementation → Hardware Testing → Verification → Project Documentation**

---

## Acknowledgement

This project was completed as part of the **B.S. in Electronic Systems** laboratory coursework at the **Indian Institute of Technology Madras**.

The hardware implementation, breadboard assembly, testing, project documentation, photographs, and demonstration videos are my original work. Laboratory reference material provided during the course was used solely for learning and understanding the concepts.

---

## Author

**Aditya Ojha**

**B.S. Electronic Systems**
Indian Institute of Technology Madras

**B.Tech Electronics & Telecommunication Engineering**
Jabalpur Engineering College

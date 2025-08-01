# IR-Remote-control
Open-Lab Project
# Problem Statement
In many modern electronic applications, remote control plays a vital role in enabling wireless device operation. Traditional remote control systems typically depend on microcontrollers, which increases system complexity. To address these limitations, we developed a six-channel IR remote control system using only analog components, eliminating the need for microcontrollers. This approach simplifies the circuit design and offers a cost-effective and efficient alternative for basic remote-control applications.
# Objective
This project aims to design and implement a simple IR remote control system without a microcontroller. The system should be capable of transmitting multiple control signals using an IR transmitter and decoding them using an IR receiver. The system was integrated into PCBs for stability and performance.
#🔧 Approach / Design / Methodology
#📡 Signal Transmission
An IR LED transmits pulse signals corresponding to different buttons on the remote.

A 555 Timer is configured to generate modulated pulses for IR transmission, ensuring proper encoding of control signals.

#📥 Signal Reception & Decoding
The IR receiver module (1838B) detects incoming IR pulses and demodulates the signal.

The demodulated signal is fed to a CD4017 decade counter, which sequentially activates outputs based on the received signal pattern, effectively decoding the input.

#⚙️ Output Control
The decoded outputs from the CD4017 are used to control multiple switching channels (up to 6).

Each channel corresponds to a dedicated button on the remote, allowing independent control of six different devices or functionalities.

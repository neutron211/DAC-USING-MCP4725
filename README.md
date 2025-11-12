# DAC-USING-MCP4725
Learn how to use the MCP4725 12-bit I²C DAC module with Arduino to generate precise analog voltages and waveforms. Includes wiring diagrams, Arduino sketches, and documentation.
MCP4725 Arduino DAC Demo
Generate smooth analog voltages and waveforms using the MCP4725 12-bit I²C DAC with an Arduino Nano.
This project demonstrates how to interface and control the MCP4725 to output DC, sine, and triangle waveforms using 5V logic.

🔧 Features
12-bit DAC resolution (4096 steps)
I²C communication
Ramp, Sine, and Triangle waveform examples
Tested on Arduino Nano (5V logic)
🧠 About MCP4725
The MCP4725 is a 12-bit Digital-to-Analog Converter (DAC) that uses the I²C bus to output true analog voltages (0–VCC).
It is perfect for:

Waveform generation
Voltage control
Analog signal simulation
⚙️ Hardware Setup
MCP4725 Pin	Arduino Nano Pin	Description
VCC	5V	Power supply
GND	GND	Common ground
SDA	A4	I²C Data
SCL	A5	I²C Clock
Default I²C address: 0x60
Change address by wiring A0 pin to VCC (address becomes 0x63)

🧩 Components Required
Component	Quantity
Arduino Nano	1
MCP4725 DAC Module	1
Jumper Wires	4–6
Breadboard	1
(Optional) Oscilloscope or Multimeter	1
💻 Software Setup
Install Adafruit_MCP4725 library from Arduino IDE Library Manager.
Connect the hardware as shown.
Upload any .ino file from the /firmware folder.
Observe voltage/waveform output on VOUT pin of MCP4725.
🧾 Example Sketches
Example	Description
MCP4725_Demo.ino	Ramp up/down waveform
examples/sine_wave.ino	Smooth sine waveform
examples/triangle_wave.ino	Triangle waveform
examples/dc_output.ino	Fixed DC voltage output

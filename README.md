# Solar Cell Phone Charger
<h2>Description</h2>
This Arduino project is a solar cell phone charger that charges your phone when you insert money. The charger uses a solar panel to power an Arduino board, a bill validator, and a 20x4 character LCD screen. The LCD screen displays the amount of money inserted, the charging time, and the status of the charger.
<h2>Prerequisites</h2>
You will need the following hardware to run this project:<br><br>

- An Arduino board (tested on an Arduino UNO)<br>
- A bill validator module (tested on a JY-926)<br>
- A 20x4 character LCD screen with an I2C interface<br>
- A solar panel (tested on a 5W panel)<br>
- A 12V battery (tested on a 7Ah lead-acid battery)<br>
- A 12V voltage regulator (tested on an LM7805)<br>

You will also need the following software:<br>

- Arduino IDE (tested on version 1.8.15)<br>
- LiquidCrystal_I2C library (tested on version 1.1.2)<br>
<h2>Installing</h2>
1. Connect the bill validator module to the Arduino board's A0 pin.<br>
2. Connect the LCD screen to the Arduino board's I2C pins (A4 for SDA and A5 for SCL).<br>
3. Connect the solar panel and the 12V battery to the voltage regulator's input pins.<br>
4. Connect the voltage regulator's output pin to the Arduino board's VIN pin.<br>
5. Open the <b>'Solar_Cell_Phone_Charger.ino</b> sketch in the Arduino IDE.<br>
6. Install the LiquidCrystal_I2C library if you haven't already (Sketch > Include Library > Manage Libraries).<br>
7. Upload the sketch to the Arduino board.<br>
<h2>Usage</h2>
1. Insert money into the bill validator module. The LCD screen will display the amount of money inserted and the charging time.<br>
2. Press the button connected to pin A2 to start the charging process. The LCD screen will display the charging time countdown.<br>
3. Once the charging time is up, the charger will stop charging and wait for more money to be inserted.<br>
<h2>License</h2>
This code is licensed under the MIT License. See the LICENSE file for details.

This code will work for an Arduino Uno R4 WiFi and is designed to be used with a Fluid'O'Tech FG304 gear pump. Contact me if you'd like a new but unwarrantied FG304 (bought a lot of these whhen I found them at a discount): jared.bandel@colorado.edu.

To use with other Arduinos, remove the "matrix" references (referring to the LED matrix on an Uno R4). Additionally, if your Arduino has no DAC, you will need to change the code referencing DAC to a PWM pin and reference it instead. There should be no difference in the pump speed between DAC and PWM values for other 5v Arduinos.

A 2021 Acaia Lunar will automatically connect to the Arduino. Make sure the Lunar firmware is up to date using the Acaia Updater app.
NOTE: After uploading the code to the Arduino, make sure to do a full power down or the Lunar will not connect. Do not just upload and wait for a reset - a power cycle is required after this!

PCBs, a wireless ESP32 screen with a full UI, mechanical parts, wiring kits and hydraulics kits are in the works. This is still a work in progress and getting it to all work together has been a major undertaking.

Arduino Uno R4 WiFi Pinout:
A0 = DAC to Pump (orange wire)
A1 = OEM 120 V Pump Wire Monitor (uses optocoupler)
A2 = Pressure sensor
A3 = Potentiometer
A4 = Screen SDA
A5 = Screen SCL
D2 = Gicar Flow Meter
D3 = Pump Tachometer (yelllow wire)
D4 = Screen SDCS (not currently required)
D5 = Autofill Monitor (uses optocoupler)
D6 = New Microswitch (normally closed, can swap wires and code for normally open if preferred)
D7 = New Relay
D8 = OEM Autofill Monitor
D9-D13 = Current touchscreen

More info coming soon!

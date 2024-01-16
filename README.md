This code will work for an Arduino Uno R4 WiFi and is designed to be used with a Fluid'O'Tech FG304 gear pump. To use with other Arduinos, remove the "matrix" references (referring to the LED matrix on an Uno R4). Additionally, if your Arduino has no DAC, you will need to change the code referencing DAC to a PWM pin and reference it instead. There should be no difference in the pump speed between DAC and PWM values.

A 2021 Acaia Lunar will automatically connect to the Arduino. Make sure the Lunar firmware is up to date using the Acaia Updater app.
NOTE: After uploading the code to the Arduino, make sure to do a full power down or the Lunar will not connect. Do not just upload and wait for a reset - a power cycle is required after this!

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
D9-D13 = Screen

PCBs, mechanical parts and wiring kits are in the works now and will be available for purchase from WE Coffee Co to make installation very easy. An ESP32 wireless screen is also in the works to clean everything up.

Any 1/4" BSP 0-200 PSI pressure sensor should work well. This is the one I'm using:
https://www.amazon.com/gp/product/B07KJJXYCJ/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

Flow meter is a standard Gicar flow meter with the 1.15 mm jet. If you have a different version, an adjustment to the calculations will be required. This is the one I'm using:
https://www.espressoparts.com/products/gicar-1-4-standard-flowmeter?variant=37555267272891&currency=USD&utm_medium=product_sync&utm_source=google&utm_content=sag_organic&utm_campaign=sag_organic&utm_source=Google&utm_medium=cpc&utm_campaign=Pmax-Everything-Else&gad_source=1&gclid=CjwKCAiAzJOtBhALEiwAtwj8tgTjSdGZb_Zka_DQnhIsd0Js7WPd022irA1rzuDbgT_ed3gP72gdrRoCBmkQAvD_BwE

More info coming soon!

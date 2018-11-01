# Control Clas Ohlson CO/Tech (Cotech) 433.92MHz power plugs from Arduino

https://www.clasohlson.com

RemoteCapture.ino by Øyvind Haga: https://www.instructables.com/id/Control-CoTech-Remote-Switch-With-Arduino-433Mhz/


# How to use
1. Load up RemoteCapture.ino and plug a 433.92MHz receiver to digital pin 2.
2. Open up Tools -> Serial Monitor in Arduino IDE and start pressing buttons from your original remotes. Note that each button sends 4 different codes and at least 2 of them are needed.
3. Copy paste the 24 bit commands to COTech.ino for sendCOTechCommand().


# How to use with example commands
1. Set the plug into pairing mode by holding down its power button until the LED starts blinking.
2. Send a command, eg. "sendCOTechCommand(SWITCH_A_ON);", which stops the pairing mode.
3. Now you can control the plug, e.g. sendCOTechCommand(SWITCH_A_ON); (or SWITCH_A_OFF).

# ESP8266 Deauther
Deauthentication attack and other hacks using an ESP8266.

This is fork of [this project](https://github.com/spacehuhn/esp8266_deauther).
I added support of PCD8544 instead of OLED display, but saved interface like it was. Also i added possibility of beacon attack from display, and going to add new functions.

# Connecting to PCD8544
So, if you want use my code, there is a pins, what i used. I connected it with nodeMCU.
```
USB TTL     NodeMCU     Nokia 5110  Description
            ESP8266     PCD8544
 
 
            GND         GND         Ground
            3V          VCC         3.3V from NodeMCU to display
            14          CLK         Output from ESP SPI clock
            13          DIN         Output from ESP SPI MOSI to display data input
            12          D/C         Output from display data/command to ESP
            #5          CS          Output from ESP to chip select/enable display
            #4          RST         Output from ESP to reset display
	    
	    #3 / D9     Up button
	    #2 / D4     Set button
	    #1 / D10    Down button
```

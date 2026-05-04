# RF-Stresser-High-Cycle-SPI-Driver
ESP32 based code for RF stresser using SPI 

Author - DoomNuke aka DP

-----------------------------------------------

The code has not been tested yet,
it is for educational purposes only

-----------------------------------------------

Disclaimer - The code hasn't been checked on an logic analyzer.

The code is not POSIX based, it has been tested on a LilyGO,

This code uses safe dBm levels - dBm level of 20 which is authorized under the FCC.

This code is made to stress RF signaling using the most amount of power, in the least amount of time,
using signal bandwidth of 500 khz which is max, frequency of 868, using AXP192 which is the power management unit,
to optimize power consumption and also managing energy in the most efficient way.

It sends bursts each 20 microseconds of data for 10 seconds and cools down for 30 seconds 
using FreeRTOS vTaskDelay.

-----------------------------------------------


The code sits under:

destroyer_headers/T-Beam_config.h -> Holds all of the configuration headers and function declarations

destroyer_source/T-Beam_config.c -> just some more init stuff for SPI driver. (cool stuff)

destroyer_source/destroyer_main.cpp -> Holds all of the logic, almost each line has an explanation of what it does exactly.

main/main.c -> Just holds the main loop where the code is ran from.


-----------------------------------------------

The code is written in C.


More to come soon :)

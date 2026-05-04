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

The code is written in C.


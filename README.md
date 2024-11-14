# Bmp280 i2c driver Implementation for stm32
## Short Overview Of the Code
Let‘s give a short overview to the code as well So how the code is written is , Separate files for bmp280 sensor driver , that is , the header file and source file . The header file
contains the interface or function prototypes and some constant definitions represents addresses of registers to communicate with the sensor. First of all Initialize function is
called from main.c file which tests the sensor , if it is correctly working ,if yes then after some additional testing I do some basic configuration as discussed earlier by writing to
the registers of bmp280 sensor.
After this I get the raw data and then convert it into the real temperature data (used some bit manipulation and callibrations) which is later used for visualization .

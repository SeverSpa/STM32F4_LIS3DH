# STM32F4_LIS3DH
STM32F4 Discovery SPI communication with the on-board accelerometer LIS3DH
1. Description
Reads with SPI the LIS3DH accelerometer on the STM32F4 Discovery board, in blocking mode, the 8 high bits for x and y, 200 reads per second. If the board is tilt , the corresponding user led is lit. The values of x and y are sent by USART1, 115200/n/8/1, and may be read by the attached Labview VI, which shows the board tilting.

2. How to use
Dowload the whole content of the project.
Run the CubeMX file c10acc.ioc and generate project for IAR EWARM. Open the generated project, Download and Degug (Ctrl+R), then Go (F5). Leds function may be seen.
Run in Labview the attached VI (Afisare3D3_2020.vi), with the attached board's image (Discovery.jpg) placed in the directory D:\ or modify its path in the middle left of the Block Diagram.  

3. Software context
The project was verified using:

-STM32 Cube MX version 5.6.0

-Firmware package STM32Cube FW_F4 V1.25.0

-IAR-EWARM v 8.50.1.

-LabView 16.0(32 bits)

Notice: For other software context, some modifications may be necessary, as the future evolution of these products is unknown.

4. Hardware context
-STM32F4 -Discovery, MB997C (equipped with LIS3DH)
-CH340  TTL to USB adapter, on PB6 and PB7

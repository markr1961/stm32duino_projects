## IKS01A1-sensors
reading the 4 sensors on the X Nucleo IKS01A1  
The X-NUCLEO-IKS01A1 interfaces with the STM32 microcontroller via the I²C pins.

device  | I2C addr  | description
------- |-----------|------------
LSM6DS0 |           | 3D accelerometer (±2/±4/±8 g) + 3D gyroscope (±245/±500/±2000 dps)
LIS3MDL |           | 3D magnetometer (±4/ ±8/ ±12/ 16 gauss)
LPS25HB |           | pressure sensor, 260-1260 hPa absolute digital output barometer
HTS221  |           | capacitive digital relative humidity and temperature

### I2C scanner
I2C device found at address 0x1E  !  
I2C device found at address 0x5D  !  
I2C device found at address 0x5F  !  
I2C device found at address 0x6B  !  
--- Scan finished ---  

### [stm32duino X-NUCLEO-IKS01A1](https://github.com/stm32duino/X-NUCLEO-IKS01A1)
The X-NUCLEO-IKS01A1 library requires the following STM32duino libraries:
[STM32duino LSM6DS0](https://github.com/stm32duino/LSM6DS0)  
[STM32duino LSM6DS3](https://github.com/stm32duino/LSM6DS3)  
[STM32duino LIS3MDL](https://github.com/stm32duino/LIS3MDL)  
[STM32duino HTS221](https://github.com/stm32duino/HTS221)  
[STM32duino LPS25HB](https://github.com/stm32duino/LPS25HB)  

For more information see [MEMS X-Nucleo.md](link needed to MEMS X-Nucleo.md)

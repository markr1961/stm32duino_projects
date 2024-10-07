## X-Nucleo MEMS Inertial and Environmental Nucleo Expansion

### [X-Nucleo-IKS01A1](https://www.st.com/en/ecosystems/x-nucleo-iks01a1.html) sensors
The X-NUCLEO-IKS01A1 interfaces with the STM32 microcontroller via the I²C pins.
- LSM6DS0: MEMS 3D accelerometer (±2/±4/±8 g) + 3D gyroscope (±245/±500/±2000 dps)
- LIS3MDL: MEMS 3D magnetometer (±4/ ±8/ ±12/ 16 gauss)
- LPS25HB*: MEMS pressure sensor, 260-1260 hPa absolute digital output barometer
- HTS221: capacitive digital relative humidity and temperature
- DIL 24-pin socket available for additional MEMS adapters and other sensors (UV index)

### [stm32duino X-NUCLEO-IKS01A1](https://github.com/stm32duino/X-NUCLEO-IKS01A1)
Best example found to date!  
The X-NUCLEO-IKS01A1 is a motion MEMS and environmental sensor expansion board for the STM32 Nucleo. 
It is equipped with Arduino UNO R3 connector layout, and is designed around the LSM6DS0 3D accelerometer and 3D gyroscope, 
the LIS3MDL 3D magnetometer, the HTS221 humidity and temperature sensor and the LPS25HB pressure sensor. 
The X-NUCLEO-IKS01A1 interfaces with the STM32 microcontroller via the I²C pin, and it is possible to change the default I²C port.  
There are several examples with the X-NUCLEO-IKS01A1 library; however only one is usable w/o the IKS01A2+LSM6DS3:
    X_NUCLEO_IKS01A1_HelloWorld: This application provides a simple example of usage of the X-NUCLEO-IKS01A1 Expansion Board. 
    It shows how to display on a hyperterminal the values of all on-board MEMS and environmental sensors.  
The X-NUCLEO-IKS01A1 library requires the following STM32duino libraries:  
[STM32duino LSM6DS0](https://github.com/stm32duino/LSM6DS0)  
[STM32duino LSM6DS3](https://github.com/stm32duino/LSM6DS3)  
[STM32duino LIS3MDL](https://github.com/stm32duino/LIS3MDL)  
[STM32duino HTS221](https://github.com/stm32duino/HTS221)  
[STM32duino LPS25HB](https://github.com/stm32duino/LPS25HB)  

## 3rd party support
[Quick Start Guide](https://www.st.com/resource/en/product_presentation/x-nucleo-iks01a1_quick_start_guide.pdf) 
[Motion MEMS and Environmental Sensor Expansion Board for STM32 Nucleo](https://community.element14.com/products/devtools/product-pages/w/documents/22091/motion-mems-and-environmental-sensor-expansion-board-for-stm32-nucleo) mostly dead links.  

### Nordic Semi
based around Zephyr RTOS: https://docs.nordicsemi.com/bundle/ncs-1.7.0/page/zephyr/getting_started/index.html  
[X-NUCLEO-IKS01A1: MEMS Inertial and Environmental Multi sensor shield](https://docs.nordicsemi.com/bundle/ncs-1.7.0/page/zephyr/boards/shields/x_nucleo_iks01a1/doc/index.html)  
[This sample enables all sensors of a X-NUCLEO-IKS01A1 shield, and then periodically reads and displays data from the shield sensors.](https://docs.nordicsemi.com/bundle/ncs-1.7.0/page/zephyr/samples/shields/x_nucleo_iks01a1/README.html#x-nucleo-iks01a1-sample) no actual code, just command line.  

### embed 
- [X-NUCLEO-IKS01A1 MEMS Inertial & Environmental Sensor Nucleo Expansion Board Firmware Package](https://os.mbed.com/teams/ST/code/X_NUCLEO_IKS01A1/)  
- [X-NUCLEO-IKS01A1 - Motion MEMS and Environmental Sensors](https://os.mbed.com/components/X-NUCLEO-IKS01A1/)  
- [embed: Sensors Reader](https://os.mbed.com/teams/ST/code/Sensors_Reader/)  

### ST SW packages
[FP-SNS-MOTENV1: STM32Cube function pack for IoT node with BLE connectivity and environmental and motion sensors](https://www.st.com/en/embedded-software/fp-sns-motenv1.html)
Sample implementations available for the X-NUCLEO-IKS4A1 (or X-NUCLEO-IKS01A3), and X-NUCLEO-BNRG2A1 or NUCLEO-U575ZI-Q connected to a NUCLEO-F401RE or NUCLEO-L476RG or NUCLEO-L053R8 board

[FP-SNS-ALLMEMS1: STM32Cube function pack for IoT node with Bluetooth Low Energy connectivity, digital microphone, environmental, and motion sensors](https://www.st.com/en/embedded-software/fp-sns-allmems1.html)
Sample implementation available for STEVAL-BCNKT01V1 and STEVAL-MKSBOX1V1 boards and for X-NUCLEO-CCA02M2, X-NUCLEO-IKS4A1 (or X-NUCLEO-IKS01A3) and X-NUCLEO-BNRG2A1 connected to a NUCLEO-F446RE or NUCLEO-L476RG boards.

[FP-SNS-FLIGHT1: STM32Cube function pack for IoT node with NFC, BLE connectivity and time-of-flight sensors](https://www.st.com/en/embedded-software/fp-sns-flight1.html)
Multitarget ranging sensor application based on the VL53L3CX Time-of-Flight (ToF) sensor.  
Sample implementation available for X-NUCLEO-53L3A2 and X-NUCLEO-BNRG2A1 connected to a NUCLEO-F401RE or NUCLEO-L476RG.  

### X-Cube-MEMS1 FW packages
[Sensor and motion algorithm software expansion for STM32Cube](https://www.st.com/en/embedded-software/x-cube-mems1.html) version A2 seems to be the old supported design.  
[X-CUBE-MEMS1 Firmware Package](https://github.com/STMicroelectronics/x-cube-mems1)
X-CUBE-MEMS1 is an expansion software package for STM32Cube. The software runs 
on the STM32 and includes drivers that recognize the sensors and collect temperature, 
humidity, pressure and motion data.

#### Supported Nucleo boards
Nucleo-F401RE
Nucleo-L083RZ
Nucleo-L152RE
Nucleo-U575ZI-Q

#### X-Cube-MEMS1 v9.4.0 sensor boards
1. IKS01A2  
    L083RZ: only Log extended.
2. IKS01A3  
3. IKS02A1  

#### X-Cube-MEMS1 v9.6.0 sensor boards
1. IKS01A2  
    L083RZ: only Log extended.
2. IKS01A3  
3. IKS02A1  

#### X-Cube-MEMS1 v10.0.0 sensor boards
IKS01A3  
IKS02A1  
IKS4A1  

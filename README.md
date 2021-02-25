# DFRobot_WT61PC
- This module integrates high-precision gyroscopes, accelerometer, microprocessor of high-performance 
and advanced dynamics solves and Kalman filter algorithms that aim to quickly solve the current real-time 
movement of the module attitude.
- The data output frequency of sensor can be revised since it uses serial communication.
- The sensor measured data include acceleration, angular velocity and angle of x, y, and z. 

## Table of Contents

* [Installation](#installation)
* [Methods](#methods)
* [History](#history)
* [Credits](#credits)

## Installation

To use this library, first download the library file, paste it into the \Arduino\libraries directory, then open the examples folder and run the demo in the folder.

## Methods

```C++
  /**
* @brief Constructor 
* @param Stream Software serial port interface 
*/
  DFRobot_WT61PC(Stream *s);

/**
* @brief  Check if there is data to read 
* @return Return true, data avaiable to read; false, no data to read 
*/
  bool available(void);

/**
* @brief Revise the data output frequncy of sensor
* @param frequency, FREQUENCY_0_1HZ for 0.1Hz, FREQUENCY_0_5HZ for 0.5Hz, FREQUENCY_1HZ for 1Hz, FREQUENCY_2HZ for 2Hz, 
  //                        FREQUENCY_5HZ for 5Hz, FREQUENCY_10HZ for 10Hz, FREQUENCY_20HZ for 20Hz, FREQUENCY_50HZ for 50Hz, 
  //                        FREQUENCY_100HZ for 100Hz, FREQUENCY_125HZ for 125Hz, FREQUENCY_200HZ for 200Hz.
*/
  void modifyFrequency(uint8_t frequency);
```

## Compatibility

| MCU           | Work Well | Work Wrong | Untested | Remarks |
| ------------- | :-------: | :--------: | :------: | ------- |
| Arduino uno   |     √     |            |          |         |
| Mega2560      |     √     |            |          |         |
| Leonardo      |           |            |      √   |         |
| ESP32         |           |     √      |          |         |
|               |           |            |          |         |


## History

- Data 2020-12-03
- Version V1.0


## Credits

Written by huyujie(yujie.hu@dfrobot.com), 2020. (Welcome to our [website](https://www.dfrobot.com/))

# DFRobot_WT61PC

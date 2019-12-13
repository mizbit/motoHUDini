# motoHUDini
Firmware for motoHUD digital speedometer and instrument cluster for motorcycle. Based on STM32F103 micro, 2.8in LCD on ILI9341 SPI driver and X27.168 dial gauge stepper motor

Written with CubeIDE using HAL and CubeMX

90% of code is in Src/freertos.c


- PCB & schematic (https://github.com/wiciu15/motoHUDsch/)

- 3D printed enclosure ( https://github.com/wiciu15/motoHUDencl/ )

- Demo video: https://youtu.be/awKXkiaZZUE

![alt text](https://i.imgur.com/zx7ixDC.png)

# Work progress

<b>Done for now:</b>

+FreeRTOS

+TFT library and SPI configuration (slightly modified https://github.com/martnak/STM32-ILI9341 library)

+working timers and interrupts for measuring kmh and RPM

+viewing values on TFT screen

+stepper motor (x27.168) as RPM meter

+2 temperature sensors (NTC100k thermistor connected to ADC as resistive divider) - <b>voltage values in soft are incorrect - need fix!!</b>

+nice UI

+mileage, average speed etc. calculation

+EEPROM for storing data after powering off (mileage and trip) (https://github.com/firebull/STM32-EEPROM-SPI library)


<b>Work still in progress:</b>


- indicators (blinker, headlights, neutral gear)

- indicator icons/bitmaps for UI

- configuration of device parameters via computer to STM32's USB CDC peripheral (Virtual COM Port)

# acam_hw_v02_cam
PCB and Schematic of Controller board for ACAM Camera in Altium Designer <br />
The Controller consist of two part, Top and Bottom boards. The main processor is stm32f417 and it also have a  ESP32 module for WIFI communication and web server.
System control the LEDs Driver board with pca9632 chip (another board), and  Temperature of inside of the case based on  three different sensors, tmp275 chip.
It also have proximity sensor (vcnl4200) for door opening detection and outside light sensor (veml6030). The  Current and The voltage of power supply (+12V,+7V,+3.3V) is measured by INA3221 chip. <br />
The controller saves the parameters and the value on SD CARD. <br />
The system have also bootloader for SD card and WIFI uploading of firmware. because of ESP32 it also support on the air firmware upgrade of main processor, ESP firmware and webserver (SPIFF format). <br />
The firmware of main processor could be found in: <br />
Bootloader: https://github.com/softqmisg/acm_HW02_bootloader  <br />
Main Firmware: https://github.com/softqmisg/acm_HW02_min_feature <br />

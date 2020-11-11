# esp-si7021

ESP32/ESP8266 component for the Si7021 sensor, for use with the [ESP-IDF](https://github.com/espressif/esp-idf) build framework. 
(ESP8266_RTOS_SDK with ESP8266)

The ESP32/ESP8266 are versatile little IoT SoC devices that can handle a number of microcontroller tasks for automation and other projects. This component allows the device to talk with an [Si7021](https://www.silabs.com/documents/public/data-sheets/Si7021-A20.pdf) temperature and humidity sensor over the I2C bus.

The use of this component is straightfoward. If the I2C bus in use has not already been initialized, you'll need to call `si7021_init()`.  Otherwise, you'll mostly be interested in `si7021_read_temperature()` and `si7021_read_humidity()` both of which return floating point temperature values.

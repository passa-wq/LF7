# [Mikrocontroller](https://de.wikipedia.org/wiki/Mikrocontroller)
(µController, µC, MCU)

## Mikrocontroller vs [SoC](https://de.wikipedia.org/wiki/System-on-a-Chip) vs [Einplatinencomputer](https://de.wikipedia.org/wiki/Einplatinencomputer)

## [Beispiele bekannter Mikrocontrollern](https://de.wikipedia.org/wiki/Liste_von_Mikrocontrollern)
* Atmel [ATtiny, ATmega](https://de.wikipedia.org/wiki/Microchip_AVR)
  * 8bit AVR

* Espressif [ESP8266](https://de.wikipedia.org/wiki/ESP8266) ([NodeMCU](https://de.wikipedia.org/wiki/NodeMCU)), [ESP32](https://de.wikipedia.org/wiki/ESP32)
  * 32bit Wi-Fi Controller

* STMicroelectronics[STM32](https://en.wikipedia.org/wiki/STM32)
  * 32bit ARM Cortex-M

* Raspberry Pi Foundation [RP2040](https://de.wikipedia.org/wiki/RP2040)
  * 32bit ARM Cortex-M0+


## Für Mikrocontroller häufig verwendete Programmiersprachen

* C, C++ -> [Arduino Sketches](https://docs.arduino.cc/learn/programming/sketches/)
* [Rust](https://docs.rust-embedded.org/book/)
* [MicroPython](https://docs.micropython.org/en/latest/esp32/quickref.html)


## [Arduino](https://docs.arduino.cc/programming/)
* [Language Reference](https://docs.arduino.cc/language-reference/)
* [Libraries](https://reference.arduino.cc/reference/en/libraries/)
* [Beispiele](https://docs.arduino.cc/built-in-examples/)
* [Tutorials](https://docs.arduino.cc/learn/starting-guide/getting-started-arduino/) […](https://www.tutorialspoint.com/arduino/)
* [Projekte](https://projecthub.arduino.cc/), […](https://www.instructables.com/Arduino-Projects/)


## Programmer und IDEs für Arduino

* [Arduino IDE](https://docs.arduino.cc/software/ide/)
* [PlatformIO](https://platformio.org/)

```bash
git clone https://github.com/platformio/platform-espressif32.git
cd platform-espressif32/examples/arduino-wifiscan
pio run -e esp320 --target upload
pio device monitor
```


## [Simulator](https://wokwi.com/)

# co2-ampel-cube

A hardware gadget measuring air CO2 content and glowing in traffic light colors to indicate air quality.

## Most important consideration: addressable leds or 2 central drivers (red, green)?

Current sway is toward addressable because the routing can be simpler and they are small too. But if only red and green are used, the number of connections between leds are the same for central drivers...

## Table of Contents

- [co2-ampel-cube](#co2-ampel-cube)
  - [Most important consideration: addressable leds or 2 central drivers (red, green)?](#most-important-consideration-addressable-leds-or-2-central-drivers-red-green)
  - [Table of Contents](#table-of-contents)
  - [Key components](#key-components)
    - [Sensirion SCD40 photoacoustic CO2 sensor](#sensirion-scd40-photoacoustic-co2-sensor)
    - [ESP32 microcontroller with wifi](#esp32-microcontroller-with-wifi)
    - [WLED software for ESP32](#wled-software-for-esp32)
    - [Addressable LED 1x1 mm](#addressable-led-1x1-mm)
  - [Mechanical Design](#mechanical-design)

## Key components

### Sensirion SCD40 photoacoustic CO2 sensor

### ESP32 microcontroller with wifi

### WLED software for ESP32

### Addressable LED 1x1 mm

XINGLIGHT XL-1010RGBC-WS2812B

## Mechanical Design

The CO2-Ampel is designed to resemble a cube with 5 faces, and all faces are printed circuit boards:

- 4 vertical surfaces with a grid of alternatingly LEDs and holes, leds facing inward
- 1 bottom surface with the sensor, USB jack, and the microcontroller facing the inside of the cube

The PCBs are fixed together by mechanically interlocking, then the gaps are bridged electrically with solder. Mechanical force is not acting on the solder joints or the lamination of the board, but the boards themselves snap into each other by having 2 tabs and one long hole on one side, and the respective opposite structure on the other side. This way, the 4 surfaces can use identical sides.

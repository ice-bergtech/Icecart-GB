# Icecart-GB

A ROM cartridge for the Gameboy.
Purpose is to fit the form factor of a gameboy cartridge and act as a ROM cartridge.
It should also have functionality similar to an arduino, where you can interface with it through GPIO.
It should be as low-power as possible, since it will run off the gameboy battery.
It should support an sd card for storage while powered off.

Requirements:

* STM32-type processor
  * low power
  * Enough pins for cart and GPIO (32+16)
  * rtc
* External mic + speaker jacks
* usb c for programming / updating
* 2x8 GPIO
* microsd card slot for storage
* 3-4MB ram
* Respond to gameboy cartridge read/write
  * 4Mihz: [gekkio notes](./reference/gbctr.pdf) appendix C [remote doc](https://gekkio.fi/files/gb-docs/gbctr.pdf)
* small battery
* gameboy dmg/color cartridge footprint (can move screw hole)
  * https://github.com/Gekkio/gb-hardware/tree/main/GB-BRK-CART


![](./block-model.png)

Schematic Snapshot: [](./schematic.pdf)
PCB Snapshot: [](./pcb.pdf)

![Schematic](./schematic.svg)

![PCB](./pcb.svg)

## Reference

emeryth-hacks: https://emeryth.net/stm32-game-boy-cartridge/

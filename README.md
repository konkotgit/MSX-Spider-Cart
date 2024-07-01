# MSX Spider Cart
Very Simple Cartridge for MSX Computers

With this PCB you can build your own MSX ROM cartridges.

You can use 8, 16 or 32kB ROM file.


# **NEW! version with flash chip. [Spider Flash Cartridge](https://github.com/konkotgit/MSX-Spider-Flash-Cart "Spider Flash Cartridge")**

## Important 

**To program the 32kB ROM correctly, you need to prepare the ROM file by swapping two 16kB blocks.**

**You can use simple windows CLI tool [swapROM](https://github.com/konkotgit/MSX-Spider-Cart/tree/main/tools "swapROM")**

The 32kB EPROM occupies address 4000h to BFFFh in the address space because it is using CS1 as read enable.

A14 will be high from 4000h to 7FFFh and low from 8000h to BFFFh. So A14 actually needs to be inverted.

By swapping the two areas no inverter is required.

## How to build cartridge

#### 27C256 EPROM (MAX 32KB ROM)

Solder only capacitor C1

**Only one of CS1, CS2 or CS12 should be closed.**

#### W27C512 EEPROM (MAX 2 x 32KB ROM)

Solder capacitor C1, resistor R1 and goldpins for JP1 jumper.

Solder goldpins for CS1, CS2 and CS12 jumper.

**Only one of CS1, CS2 or CS12 should be closed.**

Jumper JP1 must be closed on 1/2 or 2/3 position


![Spider Cart](/photos/spider_cart.jpg)

### Look at YouTube:
[![Spider Cart Youtube Video](https://img.youtube.com/vi/nXbEXRVJIhw/0.jpg)](https://www.youtube.com/watch?v=nXbEXRVJIhw)

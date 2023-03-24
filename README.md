## This project completely based on @sadkotheguest's [ch32v307-cmake-vsc-noos-template](https://github.com/sadkotheguest/ch32v307-cmake-vsc-noos-template)

# CH32V203 NoOS project template

This project provide a functional cmake/ninja project for ch32v203 MCU using standard RISC-V GCC toolchain with WCH OpenOCD support using wlinke (or wlink) debugger.

## Requeriments

 - CMake 3.16 or greater
 - ninja build tool 1.10.0 or greater
 - riscv none embed toolchain 8.2.0 or greater (from WCH or xpack provider)

## Build steps

 - Create `build` directory with `mkdir build` and move to it (`cd build`)
 - Generate cmake project using ninja (or your preferred tool): `cmake ../ -G Ninja`
 - If you prefer gnu make try `cmake ../ -G 'Unix Makefile'` (or replace to your preferred tool)
 - Launch ninja to build all of code: `ninja`
 - If all pass ok, the files `firmware.elf`, `firmware.elf.bin` and `firmware.elf.hex` appears in `build` directory
 - Additionally, you may found the files `firmware.elf.map` and `firmware.elf.lst` containing memory mapping and disassembler of the ELF file

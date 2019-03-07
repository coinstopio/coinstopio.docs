# (DRAFT) Accessing Bootloader Mode On Trezor T

**A bootloader** is a type of program that loads and starts the boot time tasks and processes of an operating system or the computer system.

  

Trezor T initialization is split into two stages. First stage boardloader is stored in write-protected area, which means it is non-upgradable. Only second stage bootloader update is allowed.

**First Stage:** [Boardloader](https://wiki.trezor.io/Boardloader "Boardloader")

**Second Stage:** Bootloader

Second stage checks the integrity and signatures of the firmware and runs it if everything is ok. If second stage bootloader detects a pressed finger on the display ([entering bootloader mode](https://wiki.trezor.io/index.php?title=User_manual%3AUpdating_your_Trezor%2527s_firmware&ModelType=2)) or there is no firmware loaded in the device, it will start in a firmware update mode, allowing a firmware update via USB.

_See also GitHub [page](https://github.com/trezor/trezor-core/blob/master/docs/bootloader.md)_
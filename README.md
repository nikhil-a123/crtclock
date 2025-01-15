# CRT Clock
A smart clock with built-in USB-C PD charging ports utilizing a readily available 4" black &amp; white CRT.

## Project Overview:

The clock is made up of three main components: the CRT module, the power board and the logic board. The power and logic board will be custom designed while the CRT module is a readily available part from Aliexpress. The three components will be integrated together in a plastic case.

## CRT

The CRT module is a 4 inch black & white CRT that accepts a composite signal. The design of the CRT is similar to ones used in the Sony Watchman line of handheld televisions, with these larger 4" types commonly used in entryphone systems in the past when LCD displays were too expensive or low quality. They can be commonly found on Aliexpress for ~£10-20. The CRT is powered by 12V and accepts a composite video signal, with optional brightness and contrast controls by attaching potentiometers.

**Link I Used:** https://www.aliexpress.com/item/1005005846819324.html

## Power Board:

The power board supplies power to the CRT and logic board and has a number of USB-C PD ports for charging devices. The power board is supplied by a USB-C PD connection.

## Logic Board

The logic board is responsible for the clock functionality, reading ambient sensors and generating composite video output to the CRT module. It uses an STM32 microcontroller for logic and a VLSI Solution VS23S010 to store the framebuffer and generate the composite video output. The logic board contains a number of different sensors to read ambient conditions such as temperature and humidity and a module to get the local time via GNSS.

## Firmware:

Note that this repository does NOT include the firmware for the STM32 microcontroller. Look at the CRT Clock firmware repository for firmware.




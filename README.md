This is one of those projects where it was a "problem" that I created. I decided that, after years of risking my life putting up Christmas lights, I was done. No, not done with Christmas lights, just the cycle. After taking inspiration from [The Hook Up](https://www.youtube.com/channel/UC2gyzKcHbYfqoXA5xbyGXtQ), and [DrZzs](https://www.youtube.com/c/DrZzs), I decided to install LED strips in a way that when they are off, you couldn't tell they were there. Where I deviated was needing to wire each strip back to a central point. I wanted a decentralized solution that only required each strip have access to 120V, and the data would come via WiFi. This is where this project starts.

# Overview

<img src="images/board_in_box.jpg" width="40%"><image src="images/pcb_assembled.jpg" width="40%">

# Details

## Purpose

The carrier board augments an ESP32 such as this one from [Amazon](https://www.amazon.com/gp/product/B086MJGFVV), or this one from [AliExpress](https://www.aliexpress.com/item/1005001757645011.html). 

The purpose of the board is:
- Interface with an ESP32
- Provide connection for bare wire, or barrel jack, from supply
- Provide connection for bare wire to LED strips
- Provide some voltage and current protection
- Step down input voltage to a level the LDO on the ESP32 can tolerate (5V)
  - The voltage regulator has the ability to run at 100% duty cycle making the carrier board 5V and 12V compatible
- Step up the data line voltage to 5V
- All fit inside a [IP68 Box](https://www.amazon.com/gp/product/B07TGHYQF4)

See included [BOM](bom.csv). It is formatted so that you may just drop it into a Digikey Cart.

<image src="images/sch.png" width="80%">

## ESP32 Firmware

For the firmware I use [WLED](https://kno.wled.ge/). If new to this I recommend starting [here](https://kno.wled.ge/basics/getting-started/).


# Materials

<image src="images/close_up_gutter.jpg" width="80%">

<image src="images/wall_mounted.jpg" width="80%">

## LED Strips
- [IP65 WS2815 12V](https://www.amazon.com/BTF-LIGHTING-Upgraded-Individually-Addressable-Non-Waterproof/dp/B07LG6KQ55)

## Hardware
- [V-Shaped Channel](https://www.amazon.com/gp/product/B07F6FKGPH) for under the gutters
- [Low Profile Channel](https://www.amazon.com/gp/product/B07KDSYLGG) for the flat surface around the garage

## Supply
- [60W IP67](https://www.amazon.com/gp/product/B07MZP9247)

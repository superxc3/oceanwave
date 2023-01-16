# Oceanwave

Oceanwave is an ergonomic unibody keyboard with 3x6 column staggered keys and 3 thumb keys designed by XCMKB. Oceanwave was inspired by [Reviung41](https://github.com/gtips/reviung/tree/master/reviung41) and [Corne](https://github.com/foostan/crkbd) additional thumb key, splayed [Architeuthis Dux](https://github.com/tapioki/cephalopoda/tree/main/Architeuthis%20dux) with mx spacing. 

![image](https://user-images.githubusercontent.com/79617315/212666136-0e20f166-bfc0-45e7-9e0f-af757469d892.png)


## Features
1. Hotswap for MX and Low Profile Choc (v1)
2. 8 RGB LED underglow 
3. 1 MX hotswap in the middle for Artisan. 
4. 1 flat wheel encoder
5. 1 EC11 / EC12 rotary encoder
6. 1 OLED
7. Pimoroni Haptic BZZZ DRV2605L Linear Actuator Haptic Breakout
8. Firmware supports wired VIAL and wireless ZMK
9. Modification of promicro or nicenano v2 for additional IOs. 
10. Power button for wireless build

## Versions
Supports multiple options of featuers for default micro controller
| Version | Features | Firmware | Wired | Wireless |
|:---|:---|:--:|:--:|:--:|
| Wirelss minimal | Flat wheel and knob | ZMK | | Yes |
| 2E | Flat wheel and knob | QMK/VIAL | Yes ||
| Oled 1E | Flat wheel or knob, Oled | QMK/VIAL | Yes ||
| Haptic 1E | Flat wheel or knob, Haptic BZZZ | QMK/VIAL | Yes ||

IO can be expanded by modifying the usb c promicro, inspired from [GOLEM](https://golem.hu/guide/pro-micro-upgrade/).
| Version | Features | Firmware | Wired | Wireless |
|:---|:---|:--:|:--:|:--:|
| Oled 2E* | Flat wheel and knob, Oled | QMK/VIAL | Yes ||
| Haptic 2E* | Flat wheel and knob, Haptic BZZZ | QMK/VIAL | Yes ||

## Build guide
[Refer here](https://github.com/superxc3/oceanwave/blob/main/build%20guide.md).

## Firmware
- QMK (link to be updated)
- ZMK

## EC11/EC12 Encoders
1. EC11 is the typical 15mm rotary encoder used for most of the mx boards, the height is almost similar to mt3. 
2. EC12 is a relatively lower height rotary encoder, used for choc board to achieve thin board thickness.  

## Keyboard Images
![image](https://user-images.githubusercontent.com/79617315/212666347-0b7923d4-43c4-4b4e-b0d7-5959e46c03e8.png)

![image](https://user-images.githubusercontent.com/79617315/212666468-71aade9f-ab0f-4c56-8582-c045f202e675.png)




## Todo
- 3D case 

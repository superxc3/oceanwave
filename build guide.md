# Build Guide of Oceanwave

### Default combination
Due to limitation of IOs, not all features can be included (4. to 7.). Below shows the combination without modifying promicro / nicenano v2

1. 1 Flat Wheel Encoder + OLED  	(join split paste for OLED on top of PCB)
2. 1 Flat Wheel Encoder + BZZZ  	(join split paste for BZZZ on top of PCB)
2. 2 Encoders, no OLED and BZZZ 	(join split paste above the flat wheel on top of PCB)

:warning: Notes

1. If do not want flat wheel as first encoder and choose ec11 rotary encoder knob, join split paste at the bottom of PCB written "JOIN IF OMIT FLAT WHEEL"
2. Once flat wheel is soldered, it must be used.
3. DO NOT SIMPLY JOIN ANYTHING IF YOU DONT USE THAT FEATURE

### Additional combination
Below shows possible combination by jump wire certain spots for additional IOs.

#### 2 Encoders + OLED or BZZZ
1. Join the ENCC and D on top of mcu (bridge wire between IO and both points)
2. Do not join split paste above the flat wheel
3. Join split paste of OLED or BZZZ depends on your choice, do not join both.

:warning: Below will lead to conflict if
1. Join OLED or BZZZ and join split paste above the flat wheel
2. Join both OLED and BZZZ

## Basic build guide

### Diodes
There are two types of diodes for oceanwave. The top facing upwards is through-hole diode; while the bottom is using SMD diode. You have to solder both types of diodes. Follow the line indicated on the pcb. 

|![image](https://user-images.githubusercontent.com/79617315/214054523-c6cf64dd-3f85-4b54-a2b8-75a484e4dd49.png)|
|:--:|
| Through-hole diode |

|![image](https://user-images.githubusercontent.com/79617315/214053728-a9102f82-0c0d-49d0-a905-a2bf30ca870b.png)|
|:--:|
| SMD diode; refer to [DIODES](https://github.com/GEIGEIGEIST/KLOR/blob/main/docs/buildguide_3DP.md#diodes) for tips to solder SMD diode |

### MCU - Microcontroller and Reset Button
The build kit comes with socket for MCU. Solder the socket and reset button after diodes. Use tape to fix the socket and solder accordingly. Default comes with usb c promicro. 

|![image](https://user-images.githubusercontent.com/79617315/214054958-0d0b25cc-2442-4b1c-a961-293c1366ec11.png)|
|:--:|
|MCU and reset button |


|![image](https://user-images.githubusercontent.com/79617315/214055949-1f84d83d-9b0f-40dd-8ba9-c1bdcd36fd56.png)|
|:--:|
| Insert the 3 pieces of 4pins at each side, put the mcu on top. Press while solder four sides of MCU, make sure no gap in between the mcu and pins. Continue to solder with the rest.|

### RGB Underglow
Apply some solder on one of the pads. Place the LED with tweezer according to the silk screen. Reheat the solder and apply some pressure with tweezer to make sure the LED is fully seated. There is an LED facing up in the middle for artisan purpose. Recommended not installed for OLED user (the led shines the oled component); and not recommended if you are not planning to insert any switch, it glares. 

|![image](https://user-images.githubusercontent.com/79617315/214058102-a35d036a-d7fc-4492-b760-87a044f79d1a.png)|
|:--:|
|Indicator silk screen. The orientation is very important. |

### Switch Sockets
Apply some solder on one of the pads, then place the switch socket and reheat the solder. While heating, press the socket with finger or tweezer. Make sure the socket is fully seated, lift your soldering iron but make sure your finger or tweezer is still pressing the socket for 1-2s. Check if the socket is aligned, then only solder the second pad. Build guide for socket and refer to [Switch Sockets](https://github.com/GEIGEIGEIST/KLOR/blob/main/docs/buildguide_3DP.md#switch-sockets).

### Encoders

#### EC11 Knob only
If you only have one encoder and prefer ec11 knob rather than flat wheel, bridge the three jumpers near to L4 RGB underglow led, above flat wheel. 

|![image](https://user-images.githubusercontent.com/79617315/214059815-b6b1aa79-4907-422d-89fb-a35bd70e7a51.png)|
|:--:|
| Join if omit flat wheel as the encoder|


|![image](https://user-images.githubusercontent.com/79617315/214064745-931d2222-535f-4a99-8b28-a379e46c171c.png)|
|:--:|
|Top: EC12 encoder with lower height, suitable for low profile choc; |
|Bottom: EC11 encoder suitable for mx choc, the height of EC11 knob is similar to the the height of MT3 keycaps.|

  :warning: The EC11 encoder allows Mill-Max 0305. However, it appears to be less stable if using Mill-Max

#### EC11 Knob and Flat Wheel
If your configuration allows you to build two encoders (both flat wheel and ec11 knob), bridge the three jumpers above the knob.

  :rotating_light: Do not bridge three jumpers above the knob to enable the knob, bridge only if you have two encoders.

|![image](https://user-images.githubusercontent.com/79617315/214060800-081b99d6-5b69-48da-a469-f84633591e43.png)|
|:--:|
| Join if your config allows for two encoders|

#### EC11 Knob and Flat Wheel with Oled and Haptic Bzzz
All enabled by expanding IO for second encoder. 
|![image](https://user-images.githubusercontent.com/79617315/218615202-2645ab4c-552c-4dfd-89b9-0c60691b9b1d.png)|
|:--:|
| Join either one of the GND, top or bottom; the another two needs to be handwired |

### OLED and Haptic Bzzz
~~Choose only OLED or Haptic Bzzz. You are allowed to bridge one of them only because they shared the same pins.~~
OLED and Haptic Bzzz are both supported as long as your firmware can fit in. 
|![image](https://user-images.githubusercontent.com/79617315/214061223-f66d9b0a-8950-46b2-9f59-72110a27ecd7.png)|
|:--:|
| Join the left 4 jumpers if choose for OLED; join the right 4 jumpers if choose for haptic bzzz. Socket for OLED on top; socket for haptic at the bottom. The photo above shows example of haptic bzzz|
|![image](https://user-images.githubusercontent.com/79617315/214062860-7d44f057-69a7-4f87-8322-fb1179fb2078.png)|
| The pins are extracted to reduce the height for socketed haptic bzzz|
|![image](https://user-images.githubusercontent.com/79617315/214063099-3aa0b4c5-c815-4199-a429-9d658f6fe985.png)|
| Silk screen explains how you should orientate the haptic bzzz, eg. GND to GND|

### Assemble
Sequence from bottom: 
1. Longer m2^4 screw at the bottom of acrylic plate
2. Acrylic bottom plate
3. Brass standsoff
4. Plastic standsoff
5. PCB
6. Shorter m2^3 screw on top of pcb

|![assemble](https://user-images.githubusercontent.com/79617315/214769087-40d48abf-56b2-45cc-bac0-80bf655e25fc.jpg)|
|:--:|
| Screws and standsoff etc |
|![Assemble - lp](https://user-images.githubusercontent.com/79617315/214771222-83940b82-30c1-4011-8d79-c771522fe248.jpg)|
| Low profile choc assemble without switch plate |
|![mx assemble](https://user-images.githubusercontent.com/79617315/214770910-e75810b1-99d9-46f0-90db-68dec6dbb903.jpg)|
| MX assemble with switch plate and oled instruction |

## Credits
Thanks for bek_jerm for pointing on knob build guide issue.


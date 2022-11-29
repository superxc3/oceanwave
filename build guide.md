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

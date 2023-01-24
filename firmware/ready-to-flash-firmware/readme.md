# Ready to flash firmware
![image](https://user-images.githubusercontent.com/79617315/214289946-4f1bd015-2ece-493f-9825-e8dbd5bd52c2.png)


## Hex for caterina promicro
Using QMK Toolbox and refer [Tutorial to flash hex file](https://github.com/superxc3/xcmkb/blob/main/list%20of%20guide/flashing%20hex.md)

## uf2 for rp2040 
Flash before soldering. Connect usb c to pc.
1. Hold the boot button on mcu, double press reset button twice. 
2. A new window pop out.
3. Drop the uf2 to the folder.
4. Done.

## Version

### Default features
- 7 layers (Layer 0123456)
- 1000Hz polling rate
- OLED/haptic depends on the build
- Mousekey availability depends on firmware size
- RGB underglow effects number depends on firmware size
- super alt tab enabled to cycle between different windows (check User tab in vial)

![image](https://user-images.githubusercontent.com/79617315/214289840-f3cf9e7f-6bb3-480e-acc9-d0c91330c05a.png)


### Oled2e
This version for OLED, without Haptic Bzzz, supports both knob and flat wheel encoders. Hex file download [here](). QMK VIAL firmware source code download [here](https://drive.google.com/drive/folders/1AIHQoCwNvRf_bx6QMLS1yq8Js87rkkeG?usp=share_link). 

Copy XCMKB and compile using `qmk compile -kb xcmkb/oceanwave -km vialoled2e`. Default comes with OLED indicator for layer, numlock, capslock, scrollock. Change the build option in oled.c for QMK logo. Animated oceanwave logo needs debug. 

**Optional features**
- mousekey disabled to accommodate rgb underglow
- qmk settings, combo, tap dance are disabled

# Firmware
Pre-assembled board is pre-flashed. Build kit please refer to [Ready-to-flash](https://github.com/superxc3/oceanwave/tree/main/firmware/ready-to-flash-firmware). If you wish to improve the codes, you will have to set up VIAL environment.

For pre-assembled and pre-flashed board, please download [VIAL](https://get.vial.today/download/) software to remap key. The software supports windows, mac, and linux. Basic layering and tapping guide refer [here](https://github.com/superxc3/xcmkb/blob/main/list%20of%20guide/vial-guide.md#basic-tapping-and-layering).

|![image](https://user-images.githubusercontent.com/79617315/214291962-a3cc96fc-744b-45f9-96bc-215382877dad.png)|
|:--:|
|Vial software interface|

## Wired QMK VIAL
- For usb-c promicro using caterina, copy xcmkb/oceanwave folder, make using `qmk compile -kb xcmkb/oceanwave -km vial`
- For rp2040 promicro, copy [oceanwave](https://drive.google.com/drive/folders/15KPRZ52J217cfi-xYsaPOL3EPukIM2lr?usp=sharing) folder to your qmk directory, make using `qmk compile -kb oceanwave -km vialoh2e`

### Configuration on Sparkfun RP2040 promicro
- Haptic vibration refers to [DRV2605L waveform library](https://github.com/qmk/qmk_firmware/blob/master/docs/feature_haptic_feedback.md#drv2605l-waveform-library); layers and tab key are added in the firmware, the rest just follow the template set in `haptic.c`.

## Wireless ZMK
Copy [oceanwave](https://drive.google.com/drive/folders/1NOylumwA9jJXKU2bHk5CELzXyPIMklsh?usp=share_link) to shields, this supports zmk-ftc only. Make using `west build -p -b nice_nano_v2 -- -DSHIELD=oceanwave`. Default keymap using reviung41 by adding extra key near to thumb. Default uf2 copy from [here](https://drive.google.com/file/d/1I9lbSuJ4-EFsmNMYBPXVArRPtXQpIEmn/view?usp=share_link). 
- no oled
- two encoders (flat wheel and rotary encoder)
- rgb included
- no haptic bzzz

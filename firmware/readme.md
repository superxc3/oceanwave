# Firmware
Pre-assembled board is pre-flashed. Build kit please refer to [Ready-to-flash](https://github.com/superxc3/oceanwave/tree/main/firmware/ready-to-flash-firmware). If you wish to improve the codes, you will have to set up VIAL environment.

For pre-assembled and pre-flashed board, please download [VIAL](https://get.vial.today/download/) software to remap key. The software supports windows, mac, and linux. Basic layering and tapping guide refer [here](https://github.com/superxc3/xcmkb/blob/main/list%20of%20guide/vial-guide.md#basic-tapping-and-layering).

|![image](https://user-images.githubusercontent.com/79617315/214291962-a3cc96fc-744b-45f9-96bc-215382877dad.png)|
|:--:|
|Vial software interface|


## Wired QMK VIAL
- For usb-c promicro using caterina, copy xcmkb/oceanwave folder, make using `qmk compile -kb xcmkb/oceanwave -km vial`
- For rp2040 promicro, copy oceanwave folder to your qmk directory, make using `qmk compile -kb oceanwave -km vial`

## Wireless ZMK

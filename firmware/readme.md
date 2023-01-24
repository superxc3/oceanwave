# Firmware
Pre-assembled board is pre-flashed. Build kit please refer to [Ready-to-flash](https://github.com/superxc3/oceanwave/tree/main/firmware/ready-to-flash-firmware). If you wish to improve the codes, you will have to set up VIAL environment.

For pre-assembled and pre-flashed board, please download [VIAL](https://get.vial.today/download/) software to remap key. The software supports windows, mac, and linux. Basic layering and tapping guide refer [here](https://github.com/superxc3/xcmkb/blob/main/list%20of%20guide/vial-guide.md#basic-tapping-and-layering).

|![image](https://user-images.githubusercontent.com/79617315/214221213-bc010371-d92d-4215-80ae-846ae0f051a7.png)|
|:--:|
|Vial software interface|


## Wired QMK VIAL
- For usb-c promicro using caterina, make using `qmk compile -kb xcmkb/oceanwave -km vial`
- For rp2040 promicro, make using `qmk compile -kb xcmkb/oceanwave/rp2040 -km vial`

## Wireless ZMK

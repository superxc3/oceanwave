# Firmware
Pre-assembled board is pre-flashed. Build kit please refer to [Ready-to-flash](https://github.com/superxc3/oceanwave/tree/main/firmware/ready-to-flash-firmware). If you wish to improve the codes, you will have to set up VIAL environment.

For pre-assembled and pre-flashed board, please download [VIAL](https://get.vial.today/download/) software to remap key. The software supports windows, mac, and linux.

## Wired QMK VIAL
- For usb-c promicro using caterina, make using `qmk compile -kb xcmkb/oceanwave -km vial`
- For rp2040 promicro, make using `qmk compile -kb xcmkb/oceanwave/rp2040 -km vial`

## Wireless ZMK

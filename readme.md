# Acer C720

This is a gist note for my Acer C720.

## Hardware

- [Heatsink Fan CPU Cooler 60.SHEN7.005](https://www.amazon.com/gp/product/B00Q3K41VA/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1)
  - If you want to replace a cooler, you will need a thermal compound paste.
- [B116XAN04.0 IPS Screen](https://s.click.aliexpress.com/e/_dULI1rF)
- [KingSpec M.2 2242 NGFF SSD](https://s.click.aliexpress.com/e/_dTuxVuV)

## Install

Remove R/W screw from the board. [Check Chromium Project page](https://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices/acer-c720-chromebook#TOC-What-s-Inside-).

Install Full ROM firmware from [MrChrmoebox.tech](https://mrchromebox.tech).

Install [Manjaro](https://manjaro.org) distro using a USB stick.

PWM fan control is not working, but it is still available to control using [`ectool`](https://aur.archlinux.org/packages/ectool-samus-git/). Note: The AUR includes ARM support which is not needed for C720.

```bash
$ git clone https://aur.archlinux.org/ectool-samus-git.git ectool
$ cd ectool && makepkg -si

# Control fan using ectool
$ ectool fanduty <0-100>
$ ectool autofanctrl
```


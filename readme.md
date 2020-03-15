# Acer C720

This is a gist note for my Acer C720.

## Install

Remove R/W screw from the board. [Check Chromium Project page](https://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices/acer-c720-chromebook#TOC-What-s-Inside-).

Install Full ROM firmware from [MrChrmoebox.tech](https://mrchromebox.tech).

Install [Manjaro](https://manjaro.org) distro using a USB stick.

PWM fan control is not working, but it is still available to control using [`ectool`](https://aur.archlinux.org/packages/ectool-samus-git/). Note: The AUR includes ARM support which is not needed for C720.

```bash
$ git clone https://aur.archlinux.org/ectool-samus-git.git ectool
$ cd ectool && makepkg -si
```


# rpi5-fan-curve
Device tree patch to improve the acoustics of the Raspberry Pi 5 Case fan curve.

# Usage
- Set up the Raspberry Pi linux kernel folliwing the instructions [here](https://www.raspberrypi.com/documentation/computers/linux_kernel.html).
- Copy `fan_curve.patch` into the `linux` repository.
- Run `git apply fan_curve.patch`
- Run `make dtbs`
- Make a backup of `/boot/firmware/bcm2712-rpi-5-b.dtb` and store it somewhere safe.
- In the `linux` repository, copy `arch/arm/boot/dts/bcm2712-rpi-5-b.dts` for a 32 bit kernel, or `arch/arm64/boot/dts/bcm2712-rpi-5-b.dts` for a 64 bit kernel, to `/boot/firmware/`.

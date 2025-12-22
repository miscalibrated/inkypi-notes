# inkypi-notes

[InkyPi](https://github.com/fatihak/InkyPi) is an open-source, customizable E-Ink display. It supports a variety of hardware configurations. Yours uses:

- [Raspberry Pi Zero 2 W](https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/).
- [WaveShare Display - 7.3 e-Paper HAT (E) - Manual](https://www.waveshare.com/wiki/7.3inch_e-Paper_HAT_(E))

There are several YouTube videos displaying the project:

- [I Built My Dream E-Ink Productivity Display](https://www.youtube.com/watch?v=UOKB9y05eOc): Latest video that provides the best overview of features
- [I built an E-Ink Calendar with a Raspberry Pi](https://www.youtube.com/watch?v=58QWxoFvtJY): Showcases waveshare hardware setup along with calendar features
- [Minimal E-Ink Clock with a Raspberry Pi (Tutorial)](https://www.youtube.com/watch?v=L5PvQj1vfC4&list=PLObZBBKx86Vvbp7zVtzGhYBe4K65B2aEz): Older video that goes over the basics of developing your own plugin
- [Full Playlist](https://www.youtube.com/playlist?list=PLObZBBKx86Vvbp7zVtzGhYBe4K65B2aEz)

Other notes and resources:

- The display flashes a bunch when refreshing, powering on/off, when updating the settings, etc. It's normal.
- Several plugins require an API key. They go in the `.env` file located in the root of the InkyPi project directory. https://github.com/fatihak/InkyPi/blob/main/docs/api_keys.md
- [More info on plugin development](https://github.com/fatihak/InkyPi/blob/main/docs/building_plugins.md)
- [Pi Zero 2 W - inkypi not updating, flashing green led](https://github.com/fatihak/InkyPi/issues/159): I didn't encounter any issues discussed in this thread, noting it here just in case.
- [AKZ Discord Server](https://discord.com/invite/qGBPVRyjCn): Developer's Discord server, if this link breaks I got it from his YouTube.
- [WaveShare Display Driver - epd7in3e](https://github.com/waveshareteam/e-Paper/blob/master/RaspberryPi_JetsonNano/python/lib/waveshare_epd/epd7in3e.py)
- Install command:

```shell
# Script takes 15-20 minutes
# Once complete you will be prompted to reboot
sudo bash install/install.sh -W epd7in3e
```

- The display flashes a bunch when refreshing. Can look like it's having an issue but it's normal.

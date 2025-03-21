# Djinn Split Keyboard

The Djinn is a 64-key split keyboard -- dual 4x7 with a 4-key thumb cluster. It also has a 5-way tactile switch under the thumb.

![Djinn](https://i.imgur.com/ArSjkv8.jpg)

Extravagance-wise, it's got audio, encoder support, per-key RGB and RGB underglow... and a 240x320 LCD. And for the safety conscious, it has ESD protection, transient voltage suppression, and polarity protection on both the USB connector as well as the split transport connector (USB-C for rev2+, TRS for rev1).

It also runs [QMK Firmware](https://qmk.fm/)!

Building can be done with:

```
make tzarc/djinn/rev2:default
```

## Rev2a

BOM: [Click](Rev2a/Djinn-BOM.md)

Fixes:

* 5-way tactile moved further away from thumb row
* Different current limiters used for RGB that are actually functional in the required range

![Djinn Rev2a PCB](https://i.imgur.com/FwygDrP.jpg)

![Djinn Rev2a PCB](https://i.imgur.com/D2tkZZf.png)

![Djinn Rev2a Built](https://i.imgur.com/xyOn5MO.jpg)

## Rev1

BOM: [Click](Rev1/Djinn-BOM.md)

![Djinn](https://i.imgur.com/iZmEG2e.jpg)

Issues:

* RGB current limiting has been reported to be problematic on Rev1 -- some builds have reported non-functional RGB without overriding the code to enable 1500mA limits
  * Measurements taken do not show that the RGB pulls anything close to 1500mA, unknown if there's a manufacturing issue or component selection issue
* 5-way tactile switch is too close to the thumb row in Rev1 and pressing in the down direction can't be achieved very easily

![Djinn Rev1 PCB](https://i.imgur.com/tDgQIRd.png)
![Djinn Rev1 PCB](https://i.imgur.com/HIBmkHB.jpg)
![Djinn Rev1 PCB](https://i.imgur.com/NRcNDYy.jpg)

---
layout: default
parent: Devices
nav_order: 0
title: Agilent 54622D
---

# {{ page.title }}

The Agilent 54622D is a 2+16 Channel, 100 MHz Mixed-Signal Oscilloscope. This product was orderable until February 28, 2007.

| Product           | Oscilloscope  |
| Status            | Obsolete      |
| Analog channels   | 2             |
| Digital channels  | 16            |
| Bandwidth         | 100 MHz       |
| Sample rate       | 200 MSa/s     |


## Gallery

![54622D]({{ page.url | append: 'img/54622D.jpg' | relative_url }})


## Documentation

| Document          | URL                                                                                   |
|:------------------|:--------------------------------------------------------------------------------------|
| User guide        | <{{ page.url | append: 'docs/User guide 9018-40677.pdf' | absolute_url }}>            |
| Programmers guide | <{{ page.url | append: 'docs/Programmers guide 9018-40679.pdf' | absolute_url }}>     |
| Service guide     | <{{ page.url | append: 'docs/Service guide 9018-40072.pdf' | absolute_url }}>         |


## Firmware

Firmware updates are performed via floppy drive. One must copy the corresponding `.jzp` file into a floppy disk, insert it into the oscilloscope and load the `.jzp` file via the `Utility` menu.

The `jzp` file format is a proprietary compression format that has been documented in <https://github.com/antoniovazquezblanco/jzp>.

| Version   | URL                                                                       |
|:----------|:--------------------------------------------------------------------------|
| A.02.31   | <{{ page.url | append: 'firmware/A.02.31/sys5462x.jzp' | absolute_url }}> |


## Modifications

### Floppy emulator

It seems there are compatible USB/SD floppy emulators. It is important to note that the connector is a flex-ribbon cable with A-B config.

Possibly compatible floppy emulator models:
* SFRC2DA
* HxC SLIM RevA ZIF 26pin

Threads referencing the mod:
* <https://groups.io/g/HP-Agilent-Keysight-equipment/topic/asking_for_recommendations_on/85046164?p=>
* <https://github.com/keirf/flashfloppy/issues/488>
* <https://github.com/keirf/FlashFloppy/issues/155>
* <https://www.eevblog.com/forum/buysellwanted/fs-(eu)-agilent-54622d/>
* <https://torlus.com/floppy/forum/viewtopic.php?t=3659>


## Compatible software

| Name                  | URL                                                                           |
|:----------------------|:------------------------------------------------------------------------------|
| Keysight IntuiLink    | <https://hackaday.io/project/171625-agilent-5460054500-extract-data-to-pc>    |
| Python script         | <https://github.com/kiwih/agilent-rs232>                                      |


## Easter eggs

### Rock on

Someone has taken the time to include an asteroids game in the scope: 
<https://www.youtube.com/watch?v=o43GDjGo7fI>


## External resources

* <https://www.keysight.com/us/en/support/54622D/portable-mso.html>


## Research topics and future work

* Can PyVISA interact with our device via RS232? <https://pyvisa.readthedocs.io/en/latest/>
* Can Sigrok interact with our device via RS232? <https://sigrok.org/wiki/Agilent_54600_Series>

# rti-performance
Performance patch for Real-Time Interaction class

## Authors:
* Philip Tovstogan
* Venkatesh Shenoy Kadandale
* Rachit Gupta

## Requirements

This patch requires the following hardware:

* LEAP motion
* 2x mobile phones

Additional software: 

* [Geco](http://uwyn.com/geco/) (Windows, Mac)
* [TouchOSC](https://play.google.com/store/apps/details?id=net.hexler.touchosc_a) (Android, iOS)

## Instructions

Make sure that LEAP motion is working well by itself on your system. To make it interact with the patch, launch GECO and use the preference file `rti.geco` in the root of this repository. The OSC output and port settings should be read from the preference file and you don't need to configure it manually.

For the phone that will be serving as a drum controller, you need to change settings in the TouchOSC app:

* switch layout to **Beatmachine**
* set port to **8003**

For the synth controller phone:

* switch layout to **Keys**
* set port to **8004**

Don't forget to set the correct OSC IP for both phones

Entry point is `main.pd` file.
This patch have been tested with *purr-data*

For any bugs and feedback, please open an issue on [github](https://github.com/philtgun/rti-performance)

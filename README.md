# KISS alyser

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Important mentions](#important-mentions)
<br><br>


## General info
Keep it simple, stupid principle based logic analyser.
```
"An idiot admires complexity, a genius admires simplicity, ..."
  -Terry A Davis
```
This project is based on the amazing work of the [fx2grok](https://sigrok.org/wiki/Fx2grok) team.<br><br>
The device we made is supposed to be a cost effective logic analyser with 16 channels. Cheap chinese analyser can be bought for less than $10 online. However, the chips are usually fake and run hot. They are also generally limited to 8 channels. This analyser can use the full 16 channels supported by the chip as long as the total sampling speed is below 192 million samples per second.
<br><br><br>


## Technologies
Project is created with:
- KiCad v5.1.12
<br><br><br>


## Setup
To use this device you will need pulseview to view and measure your connections, you can download the software [here](https://sigrok.org/wiki/Downloads).  
After the installation, plug in your analyser and start the software. It should automatically detect your device and it's capabilities. If it is not recognized, you can choose the *fx2lafw (generic driver for FX2 based LAs)* under drivers. Select USB as the connection interface and select the correct device under *Select the device*. You can now start using the logic analyser to sample data.  
You can find more information in the following links:<br><br>
pulseview manual: https://sigrok.org/doc/pulseview/0.4.1/manual.pdf  
general pulseview information: https://sigrok.org/wiki/PulseView  
supported decoders: https://sigrok.org/wiki/Protocol_decoders
<br><br><br>


## Important mentions
- Make sure to use a USB port or hub that is capable of delivering the full 480MHz needed for the device.
- The total bandwidth of the device is limited to 192 million samples per second.



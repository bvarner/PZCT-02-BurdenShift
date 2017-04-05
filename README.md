# PZCT-02-BurdenShift
Resistive burden &amp; level shift to convert PZCT-02 Split-core Current Transformer output to ADC input voltages.

In searching for split-core current transformers, I ran across this rather inexpensive solution from Amazon.
https://www.amazon.com/gp/product/B01LWN37KS/ref=oh_aui_detailpage_o04_s01?ie=UTF8&psc=1

This circuit provides burden resistance, voltage division & test point shifting to feed measurements into an Analog to Digital Converter (ADC).

I've used this with the 10bit analog input pins on Arduino's, as well as an ADS1115 16-bit ADC hooked to a raspberry pi I2C bus.

Both approaches work well. But I prefer the 16bit resolution on the I2C bus of the Pi, which can be polled rediculously fast using Collectd and the 'sensors' plugin.

# DHT22 Humidity/Temp Module Build Notes 3/3/20
 
**Design Notes:**

This module features the [DHT22 humidity/temperature sensor](https://www.sparkfun.com/datasheets/Sensors/Temperature/DHT22.pdf), also referred to as the AM2302. The pinout is as follows: 
![](https://i.imgur.com/bk8JqME.png)

On the module, the DHT22 is intended to rest perpendicular to the board.  There is a 4.7k pull-up resistor on the data line, a .1uF filtering capacitor on the VCC line, and a power indicating LED via 1k resistor. The module uses 90 degree male headers allowing for easy breadboarding.  

# Build Process
It’s easiest to solder in this order:
```
1. SMD components
2. Male headers
3. LED
4. DHT22 (bend legs before soldering)
```
**Mill Time**
	Bits: 1/32” & 1/64”: < 3mins 
	Or
	1/64” Alone: 8mins 
 
**Test**
```
1. Install the Adafruit DHT Sensor library 
2. Examples > DHT Sensor Library > DHTtester
3. Connect 5v to pin1 on the module, connect D2 (Default in example code) to pin2 on the module, and GND to pin3
4. DHT22 is the default type set in the example sketch.  Change this in the code if using a different DHTxx sensor.   
5. Upload code
6.  Open Serial Monitor 
```



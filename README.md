# TFRPM01B sensor
Revolutions per minute meter for UAV.
It is designed to direct connection to Pixhawk controller (CUAV V5+) trough standard I²C connector. The device [is supported by PX4 firmware](https://docs.px4.io/master/en/sensor/thunderfly_tachometer.html).
At the input of meter is supposed a pulse signal from optical encoder, hall sensor etc.
The hardware is inteded to be used for helicopter and autogyro rotor RPM measurement, but its counting capability is up to 20 kHz therefore it should be used for propeller or engine RPM measurement.

![Top view on I2C RPM sensor](/doc/img/TFRPM01B_top_big.jpg)

![Bottom view on I2C RPM sensor](/doc/img/TFRPM01B_bot_big.jpg)

The 3Pin probe connector is powered from I²C bus trough RC filter which limits current and voltage spikes to sensor probe.
Therefore sensor is resistant to short circuit at the probe connector power.

The two I²C Pixhawk connectors are connected to each other. This feature allows easily nesting with other I²C devices to single Pixhawks I²C port. 

### Sensor options 

The sensor could be used with multiple sensor probes. The most used one is a hall effect probe. 


![TFRPM01B hall effect magnetic sensor](/doc/img/TFRPM01B_hall_sensor.jpg)

The probe should be connected to the sensor board as follows

![TFRPM01B hall effect magnetic sensor connection](/doc/img/TFRPM01B_hall_connection.jpg)

Correct connection of the probe could be check by magnet, the PULSE LED switch on and off according to magnet presence. The sensor board needs to be powered from at least one I²C port during the test.

## Parameters

  * Pulse frequency range  0-20kHz (maximum RPM value varies by pulse number per revolution)
  * Operating and storage temperature range -20 °C  to +40 °C (limited by case material)
  * Operating input voltage range 3.6-5 V 



## Where to get it?

ThunderFly RPM counter is commercially available from [ThunderFly s.r.o.](https://www.thunderfly.cz/), write an email to info@thunderfly.cz or shop at [Tindie store](https://www.tindie.com/products/thunderfly/tfrpm01-drone-rpm-tachometer-sensor/).

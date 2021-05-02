# Hydroknecht 🌿

Hydroknecht is a smart modular 3D-printed Hydroponic system. Based on a rain-tower design it can be built to fit multiple modules with multiple planters. One planter can fit plants with a base diameter of 6 cm. The tower is controlled by multiple sensors connected to an ESP8266 wich is connected via MQTT to a Node-RED enviroment.
This enables control over pumps and lights, aswell as the reception of data from multiple analog and digital sensors. 

## Contents

- [Watering Mechanism](#watering-mechanism)
- [Modules](#modules)
- [Printing Instructions](#printing-instructions)
- [Assembly Instructions](#assembly-instructions)
- [PCB](#pcb)
- [MQTT-Commands](#mqtt-commands)
- [FAQ](#faq)


## Watering Mechanism

Hydroknecht is based on a vertical rain-tower design which is good for fast growth. Water is stored in a reservoir at the bottom of the tower from where it is pumped upwards to the top of the tower. The water at the top gets diverted and rains down onto the roots of the plants. The water is supplemented with nutrients and minerals since the plants dont have any soil to take those from. The plants themselves lie in netcups which are filled with rockwool or coconut coir which serves as a good substrate.


## Modules 

The modularity aspect of Hydroknecht allows you to design your own tower however you want. At a minimum you'll need a reservoir (or you could just use a bucket with a hole in the lid), a planter module and a shower module.

### Reservoir

The planter stores the magical water that will grow your plants. You can attach two kinds of feet to its sides. One for stability, the other for a smaller footprint. Some feet have cable ducts in them.

### Planter

This module holds the netcups in place. Available in versions for three and five netcups. The netcups are custom with an inner diameter of 63 mm.
<p>
  <img src="https://github.com/robbrobb/Hydroknecht/blob/main/documentation/planter_3.png" alt="Planter 3" width="250"/>
  <img src="https://github.com/robbrobb/Hydroknecht/blob/main/documentation/planter_5.png" alt="Planter 5" width="250"/>
</p>

### Shower

This module makes it rain. The watertube is passed through this module into the water spreader. The water is diverted by the spreader and then trickles down through the holes at the bottom.
<p>
  <img src="https://github.com/robbrobb/Hydroknecht/blob/main/documentation/shower.png" alt="Shower" width="250"/>
  <img src="https://github.com/robbrobb/Hydroknecht/blob/main/documentation/water_disperser.png" alt="Water disperser" width="250"/>
</p>

### Top

Serves as a cover and anti-splash guard. You can also place electronics here or use it as a storage place.
<p>
  <img src="https://github.com/robbrobb/Hydroknecht/blob/main/documentation/top.png" alt="Shower" width="250"/>
</p>

## Printing Instructions
The trickiest part to print is the reservoir, since this a part that you would not want leaking. You could use a bucket instead which will save you time and filament but that's not as visually appealing and might impact the stability of large towers. We suggest adding as many perimeters as you can, since that will help make the reservoir waterproof. For additional Methods have a look at [this PrusaPrinters Blog Post](https://blog.prusaprinters.org/watertight-3d-printing-pt1-vases-cups-and-other-open-models_48949/).

## Assembly Instructions

The modules are stackable and should bond together pretty neat without much force. If you want to secure the connection additionally, you can screw the modules together with an M3 Screw and Nut.


## PCB 

## MQTT-Commands
Pump Control
```bash
pump on           #turns the pump on
pump off          #turns the pump off
pump status       #returns the status of the pump over mqtt
```
Analog Sensor
```bash
analog            #returns the value of the currently connected analog sensor over mqtt
```
BME280 Sensor
```bash
bme280 temp       #returns the temperature of the bme280 sensor over mqtt
bme280 pressure   #returns the temperature of the bme280 sensor over mqtt
bme280 altitude   #returns the estimated altitude of the bme280 sensor over mqtt
bme280 humidity   #returns the humidity of the bme280 sensor over mqtt
```
Halo Control
```bash
halo on           #turns the halo on
halo off          #turns the halo off
```

## FAQ

### What's up with that name anyway?
Hydro stands for Water, Knecht is the german word for a farm labourer. So Hydroknecht means Water-Farm-Labourer, sort of .. 

### What are my minimum requirements for using Hydroknecht
A bucket of water, a 3D-printer and a remote controlled power plug with a pump will get you somewhere. Oh, and plants. Lots of plants. 🌿

## Future Stuff
- Advanced documentation and PCB Files
- Advanced base wich will allow you to use any kind of bucket as reservoir

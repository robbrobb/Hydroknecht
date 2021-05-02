# Hydroknecht 🌿

Hydroknecht is a smart modular 3D-printed Hydroponic system. Based on a rain-tower design it can be built to fit multiple modules with multiple planters. One planter can fit plants with a base diameter of 6 cm. The tower is controlled by multiple sensors connected to an ESP8266 wich is connected via MQTT to a Node-RED enviroment.
This enables control over pumps and lights, aswell as the reception of data from multiple analog and digital sensors. 

## Contents

- [Watering Mechanism](#watering-mechanism)
- [Modules](#modules)
- [PCB](#pcb)
- [MQTT-Commands](#mqtt-commands)
<li>Modules </li>
<li>Differences between smart and common version </li>
<li>The reservoir </li>
<li>Electronics </li>
<li>Components </li>
<li>Assembly </li>
<li>Slicer settings </li>

</ul> 


## Watering Mechanism

<img src="https://user-images.githubusercontent.com/82802996/116686545-40b8ea80-a9b4-11eb-888d-db138a499990.png" width="20%">

Hydroknecht is based on a vertical rain-tower design which is supposably good for fast growth. Water is stored in a reservoir at the bottom of the tower from where it is pumped upwards to the top of the tower. The water at the top gets diverted and rains down onto the roots of the plants. The water is supplemented with nutrients and minerals since the plants dont have any soil to take those from. The plants themselves lie in netcups which are filled with rockwool or coconut coir which serves as a good substrate.


## Modules 

The modularity aspect of Hydroknecht allows you to design your own tower however you want. At a minimum you'll need a reservoir (or you could just use a bucket with a hole in the lid), a planter module and a shower module.

### Reservoir

The planter stores the magical water that will grow your plants. You can attach two kinds of feet to its sides. One for stability, the other for a smaller footprint. Some feet have cable ducts in them.

### Planter

This module holds the netcups in place. Available in versions for three and five netcups. The netcups are custom with an inner diameter of 63 mm.

### Shower

This module makes it rain. The watertube is passed through this module into the water spreader. The water is diverted by the spreader and then trickles down through the holes at the bottom.

### Top

Serves as a cover and anti-splash guard. You can also place electronics here or use it as a storage place.

## PCB 

## MQTT-Commands

## Assembly Instructions

You stack them staggered so alway the first module and then the second and onand on. The angled parts are glue on the standard module. They hold the netcups in place.

So the reservoir is a little bit tricky. You must get it water safe that it not leak. You can also use a bucket which helps to safe time and filament but you dont get the overall 
iconic look for the Hydroponicsystem, also the stability is bad with huge towers so we decided to print it. You need to change a few things in prusa slicer. Prusa did a great Blog post about this theme. Here is  a link to it . [Blog Post](https://blog.prusaprinters.org/watertight-3d-printing-pt1-vases-cups-and-other-open-models_48949/)
Also a great way to get water safe results is epoxy resin. It is a bit anoying to handle but it works good for make your reservoir water safe. The best options to smooth it with 
chemicals like acetone. More Information about Water safe 3d prints are in the helpful blog post from prusaprinters.

## FAQ

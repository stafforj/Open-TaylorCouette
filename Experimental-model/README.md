# Build instructions

This section presents the concept, physical construction, wiring, and device assembly for a low-cost Taylor-Couette flow visualisation experiment. 

## Concept

The device concept was based on a number of requirements:

- Create a Taylor-Couette experiment that is accessible, low-cost and affordable (a target of under £50 was set)
- Allow users to modulate flow regimes using rotational speed control of the inner cylinder
- Extend the flow parameter space further by facilitating "hot-swappable" innner cylinders (no tools required)

To achieve an affordable design, and minimise the number of parts required for manufacturing, we utilised an off-the-shelf mini food chopper appliance which can be purchased for < £15. These choppers have some of the core components for the device, including a motor and a clear outer bowl that can facilitate flow visualisation. 

The main challenges which can restrict the chopper options are: (i) if the bowl has internal baffles, these can disrupt the Taylor-Couette flow; and (ii) if the bowl has a variable diameter along its height. Therefore, the recommendation is to source a mini chopper which has a near constant bowl diameter, and which has none or very small baffle width (e.g., < 0.6 mm).  

![concept](./Images/concept.png)

Image of three components

![components](./Images/TC-all-components.png)


Image of mini chopper
![chopper](./Images/chopper.png)


## Bill of Materials

|Name               |QTY|Description                           |
|:------------------|:-:|:-------------------------------------|
|Mini food chopper|1  |Mini food chopper. There are numerous choices. This build uses a 200W Ambiano purchased from Aldi.|
|[Motor controller board](https://www.amazon.co.uk/Controller-Regulator-Digital-Voltage-Thermostat/dp/B07SW4LXY9?pd_rd_w=i6ZY2&content-id=amzn1.sym.a509abed-8ef9-4dfc-a8ff-23f245737da1&pf_rd_p=a509abed-8ef9-4dfc-a8ff-23f245737da1&pf_rd_r=1MS1KVR6EB53WHCWNNQ2&pd_rd_wg=0FrMV&pd_rd_r=423a16b8-b44b-44d0-b718-bcb65539e7d0&pd_rd_i=B07SW4LXY9&psc=1&ref_=pd_bap_d_grid_rp_0_1_ec_pd_nav_hcs_rp_5_t)|1  |Bidirectional thyristor. The one used here is rated for very high power (up to 10kW) as I already had one available. Many other options are available with lower current/power rating that can be used.|
|2 or 3-core cable|1  |No. of cores and length depending on requirements. 1.5 mm$^2$ copper cores, or selected based on current requirements.|
|M3.5 screws|4  |12 mm long, for mounting top cover of motor controller to the enclosure body.|
|Misc.|   | <ul><li>Wiring and heat shrink</li><li>Soldering Iron and solder</li><li>Glue</li><li>Electrical hand drill and drill bits</li></ul>|

## Construction
The device is constructed from a mini food chopper, modified to rotate a cylinder at controllable rotational speeds. The speed control is necessary to adjust the flow behaviour and explore the flow instabilities that emerge at different Reynolds numbers ($R$). The estimated that the total cost of this is 

![construction](./Images/construction.png)

## Wiring

Wiring diagram
![schematic](./Images/wiring-schematic.png)

Motor control unit
![motorcontrol](./Images/motor-control-unit.png)

Module enclosure and ventilation
![vents](./Images/module-vent.png)

## Device assembly

Device assembly
![assembly](./Images/device-assembly.png)






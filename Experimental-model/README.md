# Build instructions

This section presents the concept, physical construction, wiring, and device assembly for a low-cost Taylor-Couette flow visualisation experiment. 

## Concept

The basic components for a Taylor-Couette apparatus are a stationary outer cyliner, a rotating inner cylinder, and a motor to control the rotational speed of the inner cylinder. While this is a simple configuration in principle, the cost of this type of design can be significant (~£1000's). Furthermore, implementing a design which has adaptable settings such as speed and cylinder diameter adds complexity, cost, and may require extra technical assistance when disassembling/assembling the apparatus. Our device concept was based on a number of requirements:

- Create a Taylor-Couette experiment that is accessible, low-cost and affordable (a target of under £50 was set)
- Allow users to modulate flow regimes using rotational speed control of the inner cylinder
- Extend the flow parameter space further by facilitating "hot-swappable" innner cylinders (no tools required)

To achieve an affordable design, and minimise the number of parts required for manufacturing, we utilised an off-the-shelf mini food chopper appliance which can be purchased for < £15. These choppers have some of the core components for the device, including a motor and a clear outer bowl that can facilitate flow visualisation.

The main challenges which can restrict the chopper options are: (i) if the bowl has internal baffles, these can disrupt the Taylor-Couette flow; and (ii) if the bowl has a variable diameter along its height. Therefore, the recommendation is to source a mini chopper which has a near constant bowl diameter, and which has none or very small baffle width (note these baffles could be removed using a dremel tool). We chose an Ambiano mini chopper which fits this description and is shown below. The outer diamater varied from 101 mm (top) to 98 mm (base), and the four small baffles were < 0.6 mm width. Using an inner cylinder of diameter 80 mm, the fluid gap width ($d$) varied from 9 mm to 10.5 mm along the fluid height.  

The second advantage of using this type of appliance is it allowed straightforward integration of the "hot-swappable" cylinder concept. Mini food choppers typically have removable inner blades to facilitate their cleaning after use. The stainless steel blades are rotated from below and held in place from above using an alignment pin attached to the lid of the bowl. We took advantage of this and created an inner cylinder which slots onto the motor shaft. This is shown in the schemtic below. The cylinder rotates about the axis and is held concentric with the outer cylinder using this alignment pin on the lid. 

![concept](./Images/concept.png)

The final design consists of three core components shown here: (i) an interchangeable inner cylinder; (ii) motor + clear outer cylinder (mini chopper); and (iii) module for controlling cylinder speed.

![components](./Images/TC-all-components.png)

Image of the mini chopper used in this build
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
The device is constructed from a mini food chopper, modified to rotate a cylinder at controllable rotational speeds.

![construction](./Images/construction.png)

## Wiring
Mini food choppers like the one used in this build have an on/off switch, a safety switch that ensures it cannot be operated without the lid in place, and a motor which rotates at a fixed speed. These components are all retained for the Taylor-Couette device. The motor is powered from mains AC voltage (240V). Variable speed is achieved by controlling the power to the motor from 0-100%, where 100% is achieved at the mains AC voltage. This was done by wiring in a bidirectional thyristor on the mains cable line before it enters the appliance. This is shown below in the wiring schematic and the assembly images (1-6) for the motor control module below. Note there is no need to disassemble the appliance casing at any point of this build. 

A heat sink is mounted to the TRIAC and is used to passively cool the device. An enclosure is used to avoid exposure to high temperatures and mount the display and power control buttons. To ensure cooling is not affected by the enclosure, the ventilation is designed to allow the user to orient the controller in any direction (horizontally or vertically) without introducing thermal issues. Note that this TRIAC controls power not speed, and we have observed that the 0-100% scale is non-linear. It is recommended to take measurements of cylinder speed (e.g. using a tachometer) to understand how the change in input power affects speed. This is, of course, essential for defining the correct Reynolds number ($Re = \omega r_i d / \nu$).   

![schematic](./Images/wiring-schematic.png)

Motor and cylinder control module
![motorcontrol](./Images/motor-control-unit.png)

Module enclosure and ventilation
![vents](./Images/module-vent.png)

## Device assembly for experiments

Four steps are involved for assembling the device prior to experiment. These are shown below (1-4). Between steps 2 and 3, the liquid is added to the vessel. Note there will be a maximum liquid level that avoids leaks (see _Concept_ schematic above). The manufacturer usually prints this on the bowl for the chopper, however, it is important to check this again for the Taylor-Couette set-up before performing experiments.

![assembly](./Images/device-assembly.png)






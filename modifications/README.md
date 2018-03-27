# Modification of the HRP platform at Örebro University

This folder describes the modifications made to the HRP platforms used at AASS, \"Orebro University. The central idea is to find enough space be able to fit a standard Intel based NUC computer inside the mower (which should allow mounting of any relatively large piece of equipment inside the mower).


## Hardware list

Below is a complete list of hardware along with references to locations where you could buy them (with a slight focus on buying them from Sweden).

* [Intel NUC6CAYH](https://www.intel.com/content/www/us/en/products/boards-kits/nuc/kits/nuc6cayh.html) - The computer used.
* [USB <-> Serial converter](https://se.rs-online.com/web/p/products/0429262) - FTDI Chip, UB232R, note that the mower wants a connection with 3.3V.
* [Serial Connector](https://www.elfa.se/en/male-cable-connectorp-te-connectivity-215083/p/14382321) - Male cable connectorP, 7-215083-8, TE Connectivity. To connect to the back-plane on the mower.
* [Battery Extension Cable](https://www.kjell.com/se/sortiment/dator-natverk/datorkomponenter/interna-kablar/strom-intern/forlangningskabel-for-p4-p98052?showOffline=True) - To extend one of the original battery cables.
* [Power Switch](https://www.elfa.se/sv/tryckvippstroemstaellarep-10-28-vdc-arcolectric-r13112blab/p/30013207) - Turn on/off the NUC computer.
* [Power Connector](https://www.elfa.se/en/power-plug-lumberg-connect-gmbh-1634-02/p/30068406) - Power DC plug that fits the NUC computer. 
* Mount bracket (3D printed) to hold the computer / batteries. Will replace the normal battery bracket.

## 3D printed computer / battery holder

This setup requires that you 3D print the following item.

![alt text][mount]

[mount]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/mount.jpeg "3D printed mounting bracket for holding the batteries and the NUC computer"

The CAD drawing is available [here](https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/mount.cadfile).


## Modifications

### Battery connection

The battery power is accessed by soldering two wires as described in the [HRP startup guide document](https://github.com/HusqvarnaResearch/hrp/blob/master/Startup%20Guide%20HRP.pdf) in the "Power Option Section" to get direct access to the batteries.

To be able to turn on and off the power an additional power switch is mounted close to the rear right wheel as shown below.

![alt text][battery_switch]

[battery_switch]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/battery_switch.jpeg "Battery switch placement"

### Serial connection

To communicate with the mower an USB <-> serial adapter is used (see the hardware list above). One of the AUX port is used with the serial connector. The following pins are connected:

| AUX (back-plane) | USB serial board |
| ------ | ------ |
| 1 (red) | 7 |
| 2 | 8 |
| 3 | 1 |

### Computer / battery mount

In order to fit the relatively large NUC box (L x W x H = 115 x 155 x 50 mm) the batteries positions needs to be changed. The original battery holder needs to be removed. Place the batteries as shown below (please also note the battery extension cable [black / yellow]).

![alt text][batteries]

The 3D printout is placed as shown below. Note that the 2 smaller holes are used to secure the NUC computer (which utilizes these holes to mount a VESA compatible plate (that is the computer needs to be mounted before the mounting bracket is mounted on the mower. The 4 countersink is for the NUC rubber support legs to get a snug fit.

![alt text][mount2]

The complete setup with the NUC computer is shown below.

![alt text][mount3]



[batteries]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/batteries.jpeg "Placement of batteries"
[mount2]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/mount2.jpeg "Placement of mounting bracket"
[mount3]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/mount3.jpeg "The complete setup"
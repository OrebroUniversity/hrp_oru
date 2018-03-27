# Modification of the HRP platform at Örebro University

This folder describes the modifications made to the HRP platforms used at AASS, \"Orebro University. The central idea is to find enought space be able to fit a standard intel based NUC computer inside the mower (which should allow mounting of any relatively large piece of equipment inside the mower).


## Hardware list

Below is a complete list of hardware along with references to locations where you could buy them (with a slight focus on buying them from Sweden).

* [Intel NUC6CAYH](https://www.intel.com/content/www/us/en/products/boards-kits/nuc/kits/nuc6cayh.html) - The computer used.
* [USB <-> Serial converter](https://se.rs-online.com/web/p/products/0429262) - FTDI Chip, UB232R, note that the mower wants a connection with 3.3V.
* [Serial Connector](https://www.elfa.se/en/male-cable-connectorp-te-connectivity-215083/p/14382321) - Male cable connectorP, 7-215083-8, TE Connectivity. To connect to the back-plane on the mower.
* [Battery Extension Cable](https://www.kjell.com/se/sortiment/dator-natverk/datorkomponenter/interna-kablar/strom-intern/forlangningskabel-for-p4-p98052?showOffline=True) - To extend one of the orginial battery cables.
* [Power Switch](https://www.elfa.se/sv/tryckvippstroemstaellarep-10-28-vdc-arcolectric-r13112blab/p/30013207) - Turn on/off the NUC computer.
* [Power Connector](https://www.elfa.se/en/power-plug-lumberg-connect-gmbh-1634-02/p/30068406) - Power DC plug that fits the NUC computer. 
* Mount bracket (3D printed) to hold the computer. Will replace the normal battery bracket.


## 3D printed computer / battery holder

This setup require that you print the following item.

![alt text][mount]

[mount]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/mount.jpeg "3D printed mounting bracket for holding the batteries and the NUC computer"




## Modifications

In order to fit the relatively large NUC box (L x W x H = 115 x 155 x 50 mm) the batteries positions needs to be changed. The original battery holder needs to be removed. Place the batteries as shown below (please also note the battery extension cable [black / yellow]).

![alt text][batteries]

[batteries]: https://github.com/OrebroUniversity/hrp_oru/blob/master/modifications/batteries.jpeg "Placement of batteries"


<p align="center">
 <img src="images/Image1.PNG">
</p>

# Welcome to the project of open source pixel bar !

The project goal is to create an Astera like Pixel bar, that is easy to build and cheap !

It work around Wemos D1 esp8266 and feature a custom shield and enclosure to plug on a aluminium profile. We are using [Wled library](https://github.com/wled/WLED) to run the project !

## List of components

- Wemos D1 microcontroller [Aliexpress](https://fr.aliexpress.com/item/1005007877904928.html?spm=a2g0o.productlist.main.1.4bd667c0TEfidm&algo_pvid=c34ee053-ded5-45b6-a7a7-0a01593a1252&algo_exp_id=c34ee053-ded5-45b6-a7a7-0a01593a1252-0&pdp_ext_f=%7B%22order%22%3A%223476%22%2C%22eval%22%3A%221%22%7D&pdp_npi=4%40dis%21EUR%212.44%212.44%21%21%212.70%212.70%21%40210385db17443728523754661ecd67%2112000042669746256%21sea%21FR%211895049685%21X&curPageLogUid=ZyYnmMF8z4aX&utparam-url=scene%3Asearch%7Cquery_from%3A)
- 8 x 3D printing insert M3, 3.5mm X 3.5mm [Aliexpress](https://www.aliexpress.com/item/1005003582355741.html?spm=a2g0o.order_list.order_list_main.22.22381802C50TZI)
- 8 x M2 4mm long Screw [Aliexpress](https://fr.aliexpress.com/item/32810872544.html?spm=a2g0o.order_list.order_list_main.16.22381802C50TZI&gatewayAdapt=glo2fra)
- WS2812B eco led strip 1M, 60 leds IP65
- Led Aluminium profile (See section below)
- Custom Shield (See section below)
- 3D print box (See section below)


### Led Aluminium profile

The led aluminiun profile should have the following shape and be 1 meter long :

<img src="images/aluminium.avif" alt="Alt Text" style="width:40%; height:auto;">

<br/>

It can be found on Amazon, but if you send me message I may get them for you cheaper as I order in bulk ! 


### Custom shield for Wemos D1

<p align="center">
 <img src="images/shield_pcb_3d.png" alt="Alt Text" style="width:30%; height:auto; margin-right:10px;">
 <img src="images/shield_pcb.png" alt="Alt Text" style="width:30%; height:auto; margin-right:10px;">
 <img src="images/shield_pcb_3d_2.png" alt="Alt Text" style="width:30%; height:auto;">
</p>

The shield consist of a simple PCB that route power from the a Barrel jack input to the Wemos D1 and to the led strip with a jst connector.

The shield can be ordered online (JLCPCB for example), you then need to solder :

- Barrel Type DC Connector  [Aliexpress](https://www.aliexpress.com/item/4001206395694.html?spm=a2g0o.order_list.order_list_main.89.571b1802pOpXx)
- 2.54mm pin connector
- Female 8 Pin Header Socket

The 4 mounting Hole H1-H4 are for mounting to the 3D Print case

The kicad project with PCB layout and schematic is available as a zip named [Wemos D1 shield.zip](https://github.com/mhlsf/Raptor-led/blob/main/Wemos%20d1%20shield.zip)

If needed, contact me, I can send you the ready to plug PCB for a small price !

### 3D print box

The box can be printed using any recent 3D printer. It features holes for M3 inserts to screw the PCB and the lid. STEP files are available here.

There is three stl, one for the box for PCB, one for the lid of the box and one for the other end of the led bar.

8 holes for M3 insert are made for fixing the PCB board and the lid.

At the bottom of the PCB box, there is a hole for passing led cable and to fix the box to the bar using a small screw.


<p align="center">
 <img src="images/Top1.png" alt="Alt Text" style="width:30%; height:auto; margin-right:10px;">
 <img src="images/Top3.png" alt="Alt Text" style="width:30%; height:auto; margin-right:10px;">
 <img src="images/Top2.png" alt="Alt Text" style="width:30%; height:auto;">
 <img src="images/Top4.png" alt="Alt Text" style="width:30%; height:auto;">
 <img src="images/Top5.png" alt="Alt Text" style="width:30%; height:auto;">
</p>


## Power 

Connect any 5V power source to the input jack and you are good to go.

#### Portable :

Most of the time I use [this cable](https://www.aliexpress.com/item/1005004886885121.html?spm=a2g0o.order_list.order_list_main.17.24f05e5b1uxWho) (you need the 5.5mm x 2.1mm version) and plug them directly to a portable battery.

On one 10 000mah portable battery, I can run two bar for around 6 hours at max brightness (depends on the effect used).

#### Fixed :

You can also buy a [5V 60A alimentation](https://www.amazon.fr/Alitove-dalimentation-WS2811-WS2812B-WS2813/dp/B08T2724SD?pd_rd_w=6WsGW&content-id=amzn1.sym.cbacdd79-a2a7-4dad-8c44-4a36464a6b2a%3Aamzn1.symc.ca948091-a64d-450e-86d7-c161ca33337b&pf_rd_p=cbacdd79-a2a7-4dad-8c44-4a36464a6b2a&pf_rd_r=MYNJJ29EYH6KA8NS1FD5&pd_rd_wg=14BZq&pd_rd_r=baf6692d-eb8d-406e-9d3d-868baf37e734&pd_rd_i=B08SVND5QD&th=1) to run multiple bar on one power supply.

Be carefull of the wire gauge and the wiring.


## Control

The leds can be controlled through Art-net with software like Resolume, QLC and other lighthing software.

You can also control them using the WLED app, you can check on their website more information about this. 

Many effect are programmed on those and thus easier to setup than a dedicated software.


## What's next ?

My goal is to keep improving on this design, here some of my next iteration : 

- Included Battery
- Accepting range of 5v to 36v
- Tools to quickly discover them on a network, change Wifi Hotspot etc
- Water resistance
- 3D printed Tools to attach them to various support
- Make video tutorial

<br/><br>

## Licence




















Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

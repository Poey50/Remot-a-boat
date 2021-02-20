# Remot-a-boat

This is for my boat kept usually on a mooring 200 miles round trip away. It gives me sensor information (house battery voltage, start voltage, temperature, humidity, and pressure) by return text and allows me to control 4 DC relays and an external A/C relay. Total cost excluding the A/C relay was around £40. Cost of the SIM is £2.50 per month from 1P Mobile. The standby current is 40 milliamps - about 1ah per day. I have a lithium pack on the boat which I keep at around 50% state of charge for longevity. One relay switches on a solar panel to increase the SOC in the days leading up to using the boat, if I need to. Another relay switches on a B2B to top up the start battery if I need to. Apologies for the name. My marketing department are on their final warning.

<a href="https://imgur.com/MMbB7z2"><img src="https://i.imgur.com/MMbB7z2.png" title="source: imgur.com" /></a>

I found this site to be the most useful guide to setting up the GSM 900. https://lastminuteengineers.com/sim900-gsm-shield-arduino-tutorial/

The GSM module I bought from Amazon came with a baud rate of 9600. That needs to be changed to 19200 to work with the code.

I used the software start-up option (which requires soldering a link on the module - as shown in the diagram and described in the tutorial) so that if the unit is temporarily disconnected the module will power up again automatically (rather than a 200 mile trip to hold down the re-set button for 1 second). The Arduino is powered from the 4.1 volt pin on the GSM module and this saves having a separate source of power to the Arduino.

<a href="https://imgur.com/JAredQp"><img src="https://i.imgur.com/JAredQpl.jpg" title="source: imgur.com" /></a>

The layout before measuring for the 3D enclosure. The flexible silicone sheathed wires make placing the components easy.

<a href="https://imgur.com/OQ47HfE"><img src="https://i.imgur.com/OQ47HfEl.jpg" title="source: imgur.com" /></a>

Mounted in the finished 3D printed enclosure. All connections are ready to plug into 5.5mm female jack plugs permanently installed on the boat. Relay 3 is controlling the IoT A/C Powersocket. This can also be controlled from the A/C control pin (as shown above) with a 3.5mm jack plug into the Powersocket.


PARTS

SIM900 module. (Cheaper on Chinese sites if you can bear to wait). https://www.amazon.co.uk/gp/product/B07PGKR23K/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1

Buck converter. https://www.amazon.co.uk/gp/product/B081N6WWJS/ref=ppx_yo_dt_b_asin_title_o06_s00?ie=UTF8&psc=1

Prototype shield board. (These are a little longer than strictly needed.) https://www.amazon.co.uk/gp/product/B084CX1RVY/ref=ppx_yo_dt_b_asin_title_o09_s00?ie=UTF8&psc=1

BME280. https://www.amazon.co.uk/gp/product/B07D8T4HP6/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

Dupont connectors and crimper. https://www.amazon.co.uk/gp/product/B07VQ6YNSC/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1

5 volt relays. https://www.amazon.co.uk/gp/product/B07BVXT1ZK/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=Vo

Voltage sensors. https://www.amazon.co.uk/dp/B07L81QJ75/ref=dp_prsubs_1

5.5 mm x 2.1 mm powerjack pairs of connectors. https://www.amazon.co.uk/gp/product/B077STNHRJ/ref=ppx_yo_dt_b_asin_title_o06_s00?ie=UTF8&psc=1

22 AWG silicone sheathed wires. https://www.amazon.co.uk/gp/product/B07YFXG4KX/ref=ppx_yo_dt_b_asin_title_o06_s00?ie=UTF8&psc=1

Optional Powerswitch Relay (if you want to safely operate AC). https://www.amazon.co.uk/gp/product/B0765WBGK6/ref=ppx_yo_dt_b_asin_title_o05_s00?ie=UTF8&psc=1

[img]https://i.imgur.com/JAredQpl.jpg[/img]

# Electronics Design
## components
- [Electronics refresher](https://rdorville.github.io/digfab/presentations/ep1000_electronics/ep1000_electronics.pdf)
- inventory
  - [wire](http://www.digikey.com/product-search/en?x=0&y=0&lang=en&site=us&KeyWords=AE09M-300-ND%09)
  - [button](http://www.digikey.com/product-detail/en/B3SN-3112P/SW262CT-ND)
  - [switch](http://www.digikey.com/product-detail/en/AYZ0102AGRLC/401-2012-1-ND)
  - [resistor](http://www.digikey.com/product-detail/en/RC1206FR-0710KL/311-10.0KFRCT-ND/731430): I=V/R
    - [standard values](https://www.electronics-notes.com/articles/electronic_components/resistors/standard-resistor-values-e-series-e3-e6-e12-e24-e48-e96.php)
  - capacitor: C = Q/V, I = C dV/dt
    - [unpolarized](http://www.digikey.com/product-detail/en/C3216X7R1H105K/445-1423-1-ND/569089)
    - [polarized](https://www.digikey.com/en/products/detail/panasonic-electronic-components/EEE-1EA100WR/766062)
  - [crystal](http://www.digikey.com/product-detail/en/NX5032GA-20.000000MHZ-LN-CD-1/644-1039-1-ND/1128911), [resonator](http://www.digikey.com/product-detail/en/ECS-CR2-20.00-B-TR/XC1109CT-ND/813347)
  - [inductor](http://www.digikey.com/product-detail/en/ELL-CTV100M/PCD2152CT-ND/822226): V = L dI/dt
  - diode: current from anode to cathode
    - standard diodes
    - [Schottky](http://www.digikey.com/product-detail/en/BAT46ZFILM/497-5559-1-ND/1207051)
    - [Zener](http://www.digikey.com/product-detail/en/BZT52C3V3-7-F/BZT52C3V3-FDICT-ND/717854)
    - [LED](http://www.digikey.com/product-detail/en/LTST-C150CKT/160-1167-1-ND/269239)
    - [RGB LED](https://www.digikey.com/en/products/detail/sunled/XZM2CRKM2DGFBB45SCCB/5001282)
  - transistor
    - bipolar: collector, emitter, base current gain
    - [mosfet](http://www.digikey.com/product-detail/en/NDS355AN/NDS355ANCT-ND/459000): source, drain, gate resistance
  - battery, [regulator](http://www.digikey.com/product-detail/en/LM3480IM3-5.0%2FNOPB/LM3480IM3-5.0CT-ND/270751)
  - [op-amp](http://www.digikey.com/product-detail/en/AD8615AUJZ-REEL7/AD8615AUJZ-REEL7CT-ND/951443)
  - [microcontroller](https://www.digikey.com/product-detail/en/microchip-technology/ATSAMD11C14A-SSNT/ATSAMD11C14A-SSNTCT-ND)
  - [sensors](http://academy.cba.mit.edu/classes/input_devices/index.html)
  - [actuators](http://academy.cba.mit.edu/classes/output_devices/index.html)

## electronics design (EDA) tools
- Software packages
  - [Autodesk Eagle](https://www.autodesk.com/products/eagle/free-download)
  - [Kicad](https://www.kicad.org/)
  - [EasyEDA](https://easyeda.com/)
  - [Fusion 360 CAE](https://www.autodesk.com/products/eagle/blog/fusion-360-integration-eagle)
  - [Altium Circuitmaker](https://www.altium.com/circuitmaker)
  - [DesignSpark](https://www.rs-online.com/designspark/home)
  - [Fritzing](http://fritzing.org/home/)
- packages, footprint, libraries
- workflow
  - schematic entry
  - board layout
  - (auto)routing
  - simulation
  - fabrication
- design rules
- routing layers, power planes, copper pour
- libraries for this module: [fab library](https://gitlab.fabcloud.org/pub/libraries/electronics), [digikey (Kicad library)](https://www.digikey.com/en/resources/design-tools/kicad), [SnapEDA](https://www.snapeda.com/), [Sparkfun (Eagle library)](https://github.com/sparkfun/SparkFun-Eagle-Libraries), [Adafruit (Eagle library)](https://github.com/adafruit/Adafruit-Eagle-Library), [ATtiny412 eagle part](ATTINY412-SSN.lbr)

## Eagle Tutorial
- [Schematic Capture](https://learn.sparkfun.com/tutorials/using-eagle-schematic)
- [Board Layout](https://learn.sparkfun.com/tutorials/using-eagle-board-layout)
- [PCB-gcode](https://www.youtube.com/watch?v=DVKAV7udp3Y), [pcb-gcode (modified w/slice for outline milling)](https://github.com/McNugget6750/pcb-gcode)
- [Custom SMD footprints](https://learn.sparkfun.com/tutorials/designing-pcbs-smd-footprints)
- [How to create SMD-based PCBs](https://learn.sparkfun.com/tutorials/designing-pcbs-advanced-smd)
- [Fusion 360 Electronics](https://help.autodesk.com/view/fusion360/ENU/?guid=ECD-TUTORIALS)
- [Getting started with Fusion 360 Electronics](https://www.youtube.com/watch?v=eadcyToMdLg)

## Kicad Tutorial
- [Kicad Getting Started](https://docs.kicad.org/#_getting_started)
- [Beginner's Guide to Kicad](https://learn.sparkfun.com/tutorials/beginners-guide-to-kicad)
- [Arduino Pro Mini in Kicad](https://www.youtube.com/watch?v=w0Ov9XtYdCo)

## assignment
- redraw an [echo hello-world board](http://academy.cba.mit.edu/classes/embedded_programming/index.html#echo)
  - add (at least) a button and an LED (with current limiting resistor)
  - check the design rules (ERC, DRC)
  - make it
  - test it

## Echo Hello World Boards
- ATtiny45: [schematic](../images/04_t45_hello-board.png) [board](http://academy.cba.mit.edu/classes/embedded_programming/hello.ftdi.45.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/hello.ftdi.45.jpg)
- ATtiny44: [schematic](../images/04_t44_hello-board.png) [board](http://academy.cba.mit.edu/classes/embedded_programming/hello.ftdi.44.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/hello.ftdi.44.components.jpg)
- ATtiny412: [schematic](../images/04_t412_hello-board.png) [board](http://academy.cba.mit.edu/classes/embedded_programming/t412/hello.t412.echo.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/t412/hello.t412.echo.jpg)
- [Fabacademy Boards collection](http://pub.fabcloud.io/programmers/summary/)

## assignment (reference)
- [Lucas](http://fab.academany.org/2020/labs/singapore/students/enghwalucas-lim/week6.html)
- [Ting KE](http://fab.academany.org/2020/labs/singapore/students/engting-kok/exercise06.html)

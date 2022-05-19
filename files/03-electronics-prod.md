# Electronics Production
## Skills
- making PCB
- operating a CNC machine
- populating (stuffing) a PCB
- soldering
- testing PCB

## Why make PCBs?
- customized electronics to meet product requirements
- customized footprint for product
- greater reliability
- ability to prototype & iterate faster
- better product integration

## PCB fabrication
- etching
  - [lithography](https://www.4pcb.com/media/presentation-how-to-build-pcb.pdf), [transfer](https://hackaday.com/2016/09/12/take-your-pcbs-from-good-to-great-toner-transfer/)
  - [ferric/cupric chloride](https://www.instructables.com/DIY-PCB-Etching/), [ammonium/sodium persulfate](https://www.instructables.com/PCB-Etching-prototyping/)
  - [citric acid, peroxide](http://fab.academany.org/2020/labs/kamakura/students/toshiki-tsuchiyama/assignments/week04/#5-make-etching-liquid)
  - [SDS: ferric chloride etching solution](https://us.vwr.com/assetsvc/asset/en_US/id/25631107/contents)
  - [waste](https://www.nea.gov.sg/docs/default-source/our-services/management-of-hazardous-waste.pdf)
- [machining](https://www.youtube.com/watch?v=rd0R0onbfJ0)
  - machines: [LKPF Protomat S104](https://www.lpkfusa.com/products/pcb_prototyping/machines/protomat_s104/), [Stepcraft 420](https://shop.stepcraft-systems.com/stepcraft-2-420-construction-kit), [Roland SRM-20](https://www.rolanddga.com/products/3d/srm-20-small-milling-machine)
    - tools
      - US: [0.010, 1/64, 1/32](https://www.precisebits.com/products/carbidebits/precisebit-stub.asp)
      - Metric: [0.25mm, 0.4mm, 0.8mm](https://www.aliexpress.com/item/4000742206744.html?spm=a2g0o.search0303.0.0.79a54579aaGsJT&algo_pvid=30027324-f6c4-48d1-aea6-52a1ca296834&algo_expid=30027324-f6c4-48d1-aea6-52a1ca296834-8&btsid=0bb0624116036248349635672e19ec&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
      - [V-bits](https://www.aliexpress.com/item/32959716123.html?spm=a2g0o.detail.1000014.27.a0a4663eFDrF81&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.14976.194266.0&scm_id=1007.14976.194266.0&scm-url=1007.14976.194266.0&pvid=c6e7ceff-1e44-4cf0-9820-bcb9c6187503&_t=gps-id:pcDetailBottomMoreOtherSeller,scm-url:1007.14976.194266.0,pvid:c6e7ceff-1e44-4cf0-9820-bcb9c6187503,tpp_buckets:668%230%23131923%2395_668%23808%234094%23317_668%23888%233325%2310_4976%230%23194266%238_4976%232711%237538%23182_4976%233104%239653%234_4976%234052%2318550%2321_4976%233141%239887%235_668%234328%2319931%23459_668%232846%238111%23453_668%232717%237559%2384_668%231000022185%231000066059%230_668%233422%2315392%23431_4452%230%23189847%230_4452%233474%2315675%23241_4452%233098%239599%23465_4452%233564%2316062%23633)
   - fixturing: clamps, double-sided tape
   - [underlay](http://www.ysbackupboard.com/product/underlaymaterial.html)
   - orientation
   - zeroing
   - lifetime (of endmill)
   - deburring
   - cleaning
   - [climb vs conventional machining](https://vivadifferences.com/climb-milling-vs-conventional-milling/)
- [vinyl cutter](http://fab.cba.mit.edu/classes/863.17/Harvard/people/HonghaoDeng/project-3/project-3.html) [flex](http://fab.cba.mit.edu/classes/863.17/Harvard/people/HonghaoDeng/project-9/project-9.html) [encapsulation](http://fab.cba.mit.edu/classes/863.18/Harvard/people/victoria/week_04.html)
- [laser cutter](http://fabacademy.org/archives/2015/doc/fiber-laser-cutting-pcb.html)
- [printing](http://fab.cba.mit.edu/classes/863.19/CBA/people/joaowilbert/week6/)
- [sewing](http://cba.mit.edu/docs/papers/00.07.E-broidery.pdf)

## PCB materials
- rigid
  - [FR4 (epoxy glass)](https://www.mclpcb.com/fr4-guide/)
  - [FR1 (phenolic paper)](http://www.bestpcbs.com/blog/2016/08/whats-the-difference-for-fr1-fr2-fr3-and-fr4-materials/)
- flex
  - [Kapton](https://www.dupont.com/electronic-materials/polyimide-films.html), [Pyralux](https://www.dupont.com/products/pyralux-lf.html)
  - [#1 epoxy film](http://multimedia.3m.com/mws/media/37468O/3m-epoxy-film-electrical-tape-1.pdf), [#1126 copper tape](http://multimedia.3m.com/mws/media/104361O/tape-1126-copper-foil-with-conductive-adhesive.pdf)
- copper
  - 0.5 oz: 17.5 um
  - 1.0 oz: 35 um
  - 2.0 oz: 70 um

## board houses
- [Seeed](https://www.seeedstudio.com/fusion.html), [PCBWay](https://www.pcbway.com/), [JLCPCB](https://jlcpcb.com/)
- design rules
  - width/spacing (15, 25 mils)
- layers
  - [1](http://www.electronicsandyou.com/blog/single-sided-pcb.html), [2](http://www.electronicsandyou.com/blog/double-sided-pcb.html), [multi-layer](http://www.electronicsandyou.com/blog/multilayer-pcb.html)
- [mechanical, drill, solder mask, silk screen](https://learn.sparkfun.com/tutorials/pcb-basics/all)
  - vias
  - rivets, plated, blind, buried

## components
- [through-hole](https://www.build-electronic-circuits.com/through-hole-components/)
- [surface-mount](https://www.quick-pcba.com/pcb-news/types-of-smd-components.html)
- [chip-scale](https://www.techopedia.com/definition/18622/chip-scale-package-csp)

## breadboards & other alternatives
- [(solderless) breadboard](https://www.sciencebuddies.org/science-fair-projects/references/how-to-use-a-breadboard)
- [stripboard, veroboard](https://www.electronicsclub.info/stripboard.htm), [software](https://www.electroschematics.com/veroboard-design-software/)
- [perfboard](https://sfxpcb.com/how-to-use-perfboard-without-copper/)

## assembly
- [solder](https://www.digikey.com/en/products/filter/soldering-desoldering-rework-products/262)
- [eutectic](https://fctsolder.com/eutectic-solder/)
- [wetting](https://www.circuitrework.com/guides/7-1-1.html)
- flux paste, pen
- wire, paste, bar
- manual, [drag](https://www.youtube.com/watch?v=wUyetZ5RtPs), [reflow](https://www.youtube.com/watch?v=gu0v8lfLcKg), [wave](https://en.wikipedia.org/wiki/Wave_soldering)
  - [ROHS](http://ec.europa.eu/environment/waste/rohs_eee/index_en.htm) [lead-free](https://www.digikey.com/en/products/detail/chip-quik-inc/SMDSWLF-020-4OZ/2177058) [why lead-free](https://falconerelectronics.com/lead-free-leaded-solder-difference/)
- stuffing
  - component orientation
  - tacking down parts
  - bottom to top, inside to outside
  - fumes
  - washing
- [desoldering](https://www.youtube.com/watch?v=Z38WsZFmq8E)
  - [braid](https://youtu.be/Z38WsZFmq8E?t=79)
  - [vacuum](https://youtu.be/Z38WsZFmq8E?t=176)
  - [hot air](https://www.youtube.com/watch?v=77JgIqraX_I)
  - gravity
- [cutting traces, adding jumpers](http://fab.cba.mit.edu/classes/863.17/CBA/people/tomasero/index.html)
- [pick-and-place](https://www.boarditto.com/)
- [encapsulation](https://www.youtube.com/watch?v=pExbK1EE92U)

## CAM
- formats
  - [Gerber/RS-274X](https://www.vse.com/blog/2019/10/29/gerber-files-explained-understanding-their-role-in-pcb-manufacturing/)
  - [png](https://whatis.techtarget.com/definition/PNG-Portable-Network-Graphics) resolution
  - [gcode](https://www.autodesk.com/products/fusion-360/blog/cnc-programming-fundamentals-g-code-2020-update/)
- [FlatCAM](http://flatcam.org/)
- [Carbide 3D](https://carbide3d.com/apps/pcb/)
- [mods](https://skeatz.github.io/mods/) [community](http://modsproject.org/)
  - [video](http://academy.cba.mit.edu/classes/electronics_production/mods.mp4)
- trace width
  - [traces](http://academy.cba.mit.edu/classes/electronics_production/linetest.png) [board outline](http://academy.cba.mit.edu/classes/electronics_production/linetest.interior.png) 1/64" 0.010" [fiber laser](http://academy.cba.mit.edu/classes/electronics_production/fiber.jpg)
  - traces (metric): 0.4mm, 0.8mm
- gcode viewers
  - [camotics](https://camotics.org/)
  - [ncviewer](https://ncviewer.com/)

## assignment
- group assignment:
  - characterize the design rules for your PCB production process, i.e. what is the useable minimum tracewidth for your PCB production process?
  - [Group Assignment Example](http://fab.academany.org/2020/labs/singapore/group.assignments/assignment02.html)
- individual assignment:
  - make an [in-circuit programmer](http://academy.cba.mit.edu/classes/embedded_programming/index.html#programmers) by milling and stuffing the PCB,

  - test it

## [ISP Programmer Example](http://fab.cba.mit.edu/classes/863.16/doc/projects/ftsmin/index.html)
- Download firmware
   - [ISP programmer firmware source code](http://fab.cba.mit.edu/classes/863.16/doc/projects/ftsmin/fts_firmware_bdm_v1.zip)
   - [compiled firmware hex file ATtiny45](fts_firmware_t45.hex)
   - [compiled firmware hex file ATtiny85](fts_firmware_t85.hex)

- [Windows Toolchain installation](http://fab.cba.mit.edu/classes/863.16/doc/projects/ftsmin/windows_avr.html)
  1. Install git
     - [Git for Windows download link](https://git-scm.com/download/win)
  2. Install Atmel GNU toolchain
     - [Atmel GNU toolchain for Windows](https://blog.zakkemble.net/avr-gcc-builds/)
     - [AVR toolchain download (alt 1)](https://www.microchip.com/mplab/avr-support/avr-and-arm-toolchains-c-compilers)
     - [AVR toolchain (alt 2)](https://blog.zakkemble.net/avr-gcc-builds/)

  3. Install GNU Make
     - [GNU Make download link](http://fab.cba.mit.edu/classes/863.16/doc/projects/ftsmin/make-3.81.exe)
  4. Install avrdude
     - [avrdude for Windows 10 download link](https://github.com/mariusgreuel/avrdude)
  5. [Update PATH environment variable](http://fab.cba.mit.edu/classes/863.16/doc/projects/ftsmin/windows_avr.html)
  6. Install driver (libusb-win32) for your programmer
     - [Zadig software: **libusb-win32**](http://zadig.akeo.ie/)
  7. **Sanity Check**
     - Start *Git Bash* and open terminal window
     - Type *make -v* and press Enter
     - Type *avr-gcc --version* and press Enter
     - Type *avrdude* and press Enter
  8. Uploading firmware to ISP programmer
     - Compiling firmware
       - Unzip downloaded firmware to folder
       - Open Makefile in text editor. Update *MCU = attiny45* line to the correct MCU (e.g. attiny85). Save and exit.
       - Open a terminal window and navigate to the firmware folder.
       - Type *make* and press Enter. You should see the compiled firmware, *fts_firmware.hex*
     - Connect working ISP programmer to your blank ISP programmer
     - Upload firmware to your ISP programmer
       - Type *make flash* and press Enter to upload the *fts_firmware.hex* file to your ISP programmer.
       - Type *make fuses* and press Enter to program the fuse settings on the MCU.
     - Check that Windows recognizes your ISP programmer
       - Disconnect your ISP programmer board and plug it into a USB port on your notebook.
       - Open Device Manager and check if Windows recognizes your ISP programmer. It should appear as *USBtinySPI*
     - Disable the reset fuse on the MCU
       - Reconnect the programming cable to your ISP programmer for the final step (disable reset pin, make it an I/O pin)
       - Type *make rstdisbl* and press Enter
       - Congratulations. You have uploaded the ISP firmware to your programmer.
     - Check that you have the correct Windows driver
       - Plug your ISP programmer to a USB port on your notebook
       - Open Device Manager. Your programmer should appear under the *libusb-win32 device* as *USBtinySPI*
   
  - Refer to [YeoGS](http://fab.academany.org/2020/labs/singapore/students/gausiong-yeo/exercise04.html) assignment in the link below if you are unsure of the steps.

## FTDI/UPDI Example
- FTDI example: [board](../images/02_ch330n_ftdi_board.png) [components](../images/02_ch330n_ftdi_components.jpg) [trace](../images/02_ch330-ftdi_traces.png) [outline](../images/02_ch330-ftdi_outline.png)

- FTDI-to-UDPI interface board: [board](../images/03_ftdi2updi.png) [components](../images/03_ftdi2updi_components.jpg) [trace](../images/03_ftdi2updi_traces.png) [outline](../images/03_ftdi2updi_outline.png)

## ATSAMD11C Collection
- [Fab Academy Programmers](http://pub.fabcloud.io/programmers/summary/)

## Arduino ISP
- [Arduino Uno as ISP](https://create.arduino.cc/projecthub/arjun/programming-attiny85-with-arduino-uno-afb829)

## Recommended settings for Stepcraft

| Operation | Endmill size | Cut Speed | Cut Depth | Total Depth | Offset
| :--- | :---: | :---: | :---: | :---: | :---:
| Traces | 0.4 mm flat | 50 ~ 60 mm/min | 0.04 ~ 0.05 mm | 0.04 ~ 0.05 mm | 2 ~ 4
| Traces | 0.8 mm flat | 60 ~ 80 mm/min | 0.04 ~ 0.05 mm | 0.04 ~ 0.05 mm | 1 ~ 2 
| Traces | 0.1 mm 30 deg V-bit | 50 ~ 60 mm/min | 0.04 ~ 0.05 mm | 0.04 ~ 0.05 mm | 1 ~ 2
| Board Outline | 0.8 mm flat | 50 ~ 80 mm/min | 0.42 ~ 0.45 mm | 1.65 ~ 1.70 mm | 1

**Note:**
- **Safety glasses must be used when viewing milling process**
- confirm feedrate settings in G-code
- confirm z-sensor probe is activated when switch depressed
- perform an air cut or camotics simulation before beginning cutting
- perform z-calibration everyting endmill or mill bit is changed

## assignment (reference)
- [Noel](http://fab.academany.org/2020/labs/singapore/students/noel-kristian/exercise04.html)
- [Yeo GS](http://fab.academany.org/2020/labs/singapore/students/gausiong-yeo/exercise04.html)

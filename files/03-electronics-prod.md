# Electronics Production
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
   - fixturing
   - sacrificial layer
   - orientation
   - zeroing
   - lifetime (of endmill)
   - deburring
   - cleaning
   - climb vs conventional machining
- vinyl cutter flex connections encapsulation milling
- laser cutter
- printing
- plating
- sewing

## PCB materials
- rigid
  - FR4 (epoxy glass)
  - FR1 (phenolic paper)
- flex
  - Kapton, Pyralux
  - #1 epoxy film, #1126 copper tape
- copper
  - 0.5 oz: 17.5 um
  - 1.0 oz: 35 um
  - 2.0 oz: 70 um

## board houses
- Seeed, PCBWay, JLCPCB,
- design rules
  - width/spacing (15, 25 mils)
- layers
  - 1, 1.5, 2, 2+, 4, N
- mechanical, drill, solder mask, silk screen
  - vias
  - rivets, plated, blind, buried

## components
- through-hole
- surface-mount
- chip-scale

## breadboards

## assembly
- solder
- eutectic
- wetting
- flux paste, pen
- wire, paste, bar
- manual, drag, reflow, wave
  - ROHS lead-free
- stuffing
  - component orientation
  - tacking down parts
  - bottom to top, inside to outside
  - fumes
  - washing
- desoldering
  - braid
  - vacuum
  - hot air
  - gravity
- cutting traces, adding jumpers
- pick-and-place
- encapsulation

## CAM
- formats
  - Gerber/RS-274X
  - png resolution
- FlatCAM
- mods community
  - video
- trace width
  - traces interior 1/64" 0.010" fiber laser
   
## assignment
- group assignment:
  - characterize the design rules for your PCB production process
- individual assignment:
  - make an in-circuit programmer by milling and stuffing the PCB,
  - test it, then optionally try other PCB processes

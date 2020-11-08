## Embedded Programming

- architectures
  - [von Neumann](https://www.javatpoint.com/von-neumann-model), [Harvard](https://www.geeksforgeeks.org/harvard-architecture/)
  - [RISC](https://binaryterms.com/risc-processor.html), [CISC](https://binaryterms.com/cisc-processors.html)
  - microprocessor, microcontroller
  - [GPU](https://www.hellotech.com/blog/whats-a-gpu-what-gpu-do-you-have), [TPU](https://analyticsindiamag.com/tpu-beginners-guide-google/)
  - [FPGA](https://www.xilinx.com/products/silicon-devices/fpga/what-is-an-fpga.html), [TinyFPGA](https://tinyfpga.com/), [ASICs](https://www.elprocus.com/application-specific-integrated-circuits/), [difference](https://numato.com/blog/differences-between-fpga-and-asics/)

- memory
  - registers (instructions)
  - SRAM (fast)
  - DRAM (big)
  - EEPROM (non-volatile)
  - FLASH (programs, strings)
  - fuse (configuration)

- peripherals
  - ports
  - A/D
  - comparator
  - D/A
  - timer/counter/PWM
  - USART
  - USB
  - ...

- word size
  - 8
  - 16
  - 32
  - 64

- families
  - [8051](http://www.faqs.org/faqs/microcontroller-faq/8051/)
  - [PIC](https://www.microchip.com/design-centers/microcontrollers)
  - [MSP](http://www.ti.com/lsds/ti/microcontroller/16-bit_msp430/overview.page)
  - [AVR](https://www.microchip.com/design-centers/8-bit/microchip-avr-mcus)
    - [ATtiny412](https://www.digikey.com/product-detail/en/microchip-technology/ATTINY412-SSFR/ATTINY412-SSFRCT-ND),  [ATtiny45](http://www.digikey.com/product-detail/en/ATTINY45V-10SU/ATTINY45V-10SU-ND)
    - [ATtiny1614](https://www.digikey.com/product-detail/en/microchip-technology/ATTINY1614-SSNR/ATTINY1614-SSNRCT-ND), [ATtiny44](http://www.digikey.com/product-detail/en/ATTINY44A-SSU/ATTINY44A-SSU-ND)
    - [ATtiny3216](https://www.digikey.com/product-detail/en/microchip-technology/ATTINY3216-SFR/ATTINY3216-SFRCT-ND), [ATmega328](https://www.digikey.com/en/products/detail/microchip-technology/ATMEGA328PB-AU/5638812)
   - ARM
     - [D11C](https://www.digikey.com/products/en?keywords=ATSAMD11C14A-SSUTCT-ND), [D11D](https://www.digikey.com/products/en?keywords=ATSAMD11D14A-SSUTCT-ND)
   - Xtensa
     - [ESP8266](https://www.espressif.com/en/products/hardware/esp8266ex/overview)
     - [ESP32](https://www.espressif.com/en/products/hardware/esp32/overview)
   - PSoC, xCORE, Propeller, Lattice, NVIDIA
   - [RISC-V](https://cacm.acm.org/magazines/2020/5/244325-will-risc-v-revolutionize-computing/fulltext)

- vendors
  - [Octopart](http://octopart.com/)
  - [DigiKey](https://www.digikey.sg/)
  - [Mouser](https://www.mouser.sg/)
  - [RS Components](https://uk.rs-online.com/web/)
  - [Element14](https://sg.element14.com/)
  - [SparkFun]j(http://www.sparkfun.com/)
  - [Adafruit](https://www.adafruit.com/)

- [packages](https://www.microchip.com/en-us/support/package-drawings)
  - DIP
  - SOT
  - SOIC
  - TSSOP
  - TQFP
  - LQFP
  - BGA

- in-system development
  - ISP (AVR)
    - software
      - [avrdude](http://www.nongnu.org/avrdude/)
    - hardware
      - [header](http://www.mouser.com/ProductDetail/FCI/95278-101A06LF/?qs=sGAEpiMZZMtsLRyDR9nM14Vjyw4ze%252bjt4BkljYq5qeM%3d) [pads](http://academy.cba.mit.edu/classes/embedded_programming/hello.ISP.44.traces.png) [clip](http://www.digikey.com/product-detail/en/3m/923655-14/923655-14-ND) [pins](http://fab.cba.mit.edu/classes/863.16/doc/projects/Pogo_prog_connector/Pogo.html)
      - [Atmel-ICE](http://www.digikey.com/product-detail/en/ATATMEL-ICE-BASIC/ATATMEL-ICE-BASIC-ND)
      - [Arduino](https://www.arduino.cc/en/Main.ArduinoISP)
      - ATmega16U2-based ISP/PDI programmer [Zaerc](https://gitlab.fabcloud.org/FabISPmk2/FabPDI)
      - FabtinyISP: [Brian](http://fab.cba.mit.edu/classes/863.16/doc/projects/ftsmin/index.html)
  - UPDI (AVR 0,1-series)
    - software
      - [pyupdi](https://github.com/mraardvark/pyupdi)
           install: pip3 install intelhex pylint pyserial
           program: python3 pyupdi.py -d your_processor -c your_port -b your_baud_rate -f your_hex -v
      - hardware
        - [hello.serial-UPDI.FT230X](http://academy.cba.mit.edu/classes/embedded_programming/UPDI/FTDI-UPDI) [board](http://academy.cba.mit.edu/classes/embedded_programming/UPDI/FTDI-UPDI.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/UPDI/FTDI-UPDI.jpg) [traces](http://academy.cba.mit.edu/classes/embedded_programming/UPDI/FTDI-UPDI.traces.png) [interior](http://academy.cba.mit.edu/classes/embedded_programming/UPDI/FTDI-UPDI.interior.png)
        - [hello.USB-UPDI.FT230X](http://academy.cba.mit.edu/classes/embedded_programming/FTDI/USB-FT230XS-UPDI) [board](http://academy.cba.mit.edu/classes/embedded_programming/FTDI/USB-FT230XS-UPDI.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/FTDI/USB-FT230XS-UPDI.jpg) [traces](http://academy.cba.mit.edu/classes/embedded_programming/FTDI/USB-FT230XS-UPDI.traces.png) [interior](http://academy.cba.mit.edu/classes/embedded_programming/FTDI/USB-FT230XS-UPDI.interior.png)
        - [Arduino nano](https://github.com/SpenceKonde/megaTinyCore/blob/master/MakeUPDIProgrammer.md)
  - JTAG (ARM)
    - software
      - [OpenOCD]j(http://openocd.org/)
      - [EDBG](https://github.com/ataradov/edbg)
           program: edbg -b -t target_type -pv -f binary_file
           read fuses: edbg -b -t target_type -F r,*,file_name
           write fuses: edbg -b -t target_type -F w,high_bit:low_bit,bit_value
    - hardware
      - [Atmel-ICE](http://www.digikey.com/product-detail/en/ATATMEL-ICE-BASIC/ATATMEL-ICE-BASIC-ND)
      - [PICO](https://www.digikey.com/product-detail/en/maxim-integrated/MAX32625PICO/MAX32625PICO-ND/7560410)
      - [GoodFET](http://goodfet.sourceforge.net/)
      - [Raspberry Pi](https://learn.adafruit.com/programming-microcontrollers-using-openocd-on-raspberry-pi/overview)
      - [Free-DAP](https://github.com/ataradov/free-dap)
            [hello.CMSIS-DAP.10.D11C](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.10.D11C) [board](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.10.D11C.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.10.D11C.jpg) [traces](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.10.D11C.traces.png) [interior](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.10.D11C.interior.png)
            [hello.CMSIS-DAP.4.D11C](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.4.D11C) [board](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.4.D11C.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.4.D11C.jpg) [traces](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.4.D11C.traces.png) [interior](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.4.D11C.interior.png)
            [hello.SWD.10-4](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.SWD.10-4) [board](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.SWD.10-4.png) [components](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.SWD.10-4.jpg) [traces](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.SWD.10-4.traces.png) [interior](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.SWD.10-4.interior.png)
               [binary](http://academy.cba.mit.edu/classes/embedded_programming/SWD/free_dap_d11c_mini.bin) [video](http://academy.cba.mit.edu/classes/embedded_programming/SWD/hello.CMSIS-DAP.4.D11C.mp4)
   - [bootloader](https://github.com/arduino/Arduino/wiki/Unofficial-list-of-3rd-party-boards-support-urls) (all)

- assembly language
  - [hex file](http://fab.cba.mit.edu/about/fab/hello/ftdi/hello.ftdi.44.echo.hex)
  - [instruction set](http://academy.cba.mit.edu/classes/embedded_programming/doc0856.pdf), opcodes
  - [mnemonics](http://academy.cba.mit.edu/classes/embedded_programming/doc1022.pdf), [directives](http://academy.cba.mit.edu/classes/embedded_programming/doc1022.pdf), [expressions](http://academy.cba.mit.edu/classes/embedded_programming/doc1022.pdf)
  - [avr-as](http://www.nongnu.org/avr-libc/user-manual/overview.html)
  - [inline](http://www.nongnu.org/avr-libc/user-manual/inline_asm.html)

- C
  - [programming](https://gitlab.fabcloud.org/academany/fabacademy/2020/recitations/blob/master/programming.pdf)
  - [GCC](http://gcc.gnu.org/)
    -  [make files](https://www.gnu.org/software/make/manual/html_node/Introduction.html#Introduction)
    -  [bit operations](http://playground.arduino.cc/Code/BitMath)
  - AVR
    - [libc](http://www.nongnu.org/avr-libc/user-manual/index.html) [modules](http://www.nongnu.org/avr-libc/user-manual/modules.html) [types](http://www.nongnu.org/avr-libc/user-manual/group__avr__stdint.html) [math](http://www.nongnu.org/avr-libc/user-manual/group__avr__math.html) [benchmarks](http://www.nongnu.org/avr-libc/user-manual/benchmarks.html)
    - [avr-libc](http://packages.ubuntu.com/xenial/avr-libc) [binutils-avr](http://packages.ubuntu.com/xenial/binutils-avr) [gcc-avr](http://packages.ubuntu.com/xenial/gcc-avr)
    - [homebrew-avr](https://github.com/osx-cross/homebrew-avr)
  - ARM
    - [gcc-arm-none-eabi](http://packages.ubuntu.com/xenial/gcc-arm-none-eabi) [gdb-multiarch](http://packages.ubuntu.com/xenial/gdb-multiarch)
    - [homebrew-arm](https://github.com/osx-cross/homebrew-arm)
  - Microchip
    - [ASF](https://asf.microchip.com/docs/latest)
    - [Studio](https://www.microchip.com/avr-support/atmel-studio-7)
    - [toolchains](https://www.microchip.com/mplab/avr-support/avr-and-arm-toolchains-c-compilers) [packs](http://packs.download.atmel.com/)

- IDE
  - [Atmel Studio](https://www.microchip.com/avr-support/atmel-studio-7)
  - [Arduino](https://www.arduino.cc/en/Main/Software)
  - [Eclipse AVR](http://www.eclipse.org/)
  - [Firefly](http://www.grasshopper3d.com/profile/firefly)
  - [Scratch](http://wiki.scratch.mit.edu/wiki/PicoBoard)
  - [Modkit](http://www.modk.it/)

- boards
  - Atmel Adafruit Olimex Polulu MattairTech

- Arduino
  - board + toolchain + libraries + IDE + bootloader + header
  - programming
    - C++ Create Codebender Ardublock
  - original
    - Fabkit Fabio satshakit hello.328P
  - cores
    - ATtiny tinyAVR SAMD ESP8266 ESP32
  - boards
    - Adrianino

- clocks
  - types
    - RC (10%, 1% calibrated)
    - ceramic (0.5%)
    - quartz (50 ppm)
  - PLL
  - instruction cycles
  - overclocking

- host communication
  - RS232
    - bit timing
  - VT100/ANSI/ISO/ECMA terminal
    - Screen Kermit Minicom Arduino
    - pySerial minitermy
         python -m serial.tools.miniterm /dev/your_device_port your_baud_rate
    - SerialPort terminal
         serialport-terminal
  - USB
    - software
      -  V-USB
    - hardware
      - LUFA ASF Arduino
  - FTDI
    - drivers
    - libFTDI
    - cable
    - chip
      - hello.USB-serial.FT230X board components traces interior

- ATtiny412
  - hello.t412.blink board components traces interior
      timing blink.ino video
  - hello.t412.echo board componenets traces interior
      UART echo.ino video

- ATtiny45
  - hello.ftdi.45 board components traces interior pin re-use
      ports port.c port.make port.ino port.write.ino
      bit-bang echo.c echo.make echo.ino echo.serial.ino video

- ATtiny1614
  - hello.t1614.echo board components traces interior
      echo.ino video

- ATtiny44
  - hello.ftdi.44 board components traces interior
  - hello.ftdi.44.2 board components top bottom holes interior
      programming mods
      echo.c echo.c.make
      echo.interrupt.c echo.interrupt.c.make
      echo.asm echo.asm.make

- ATtiny3216
  - hello.t3216.echo board components traces interior
      echo.ino video

- ATSAMD11C
  - hello.D11C.blink board components traces interior
  - hello.D11C.blink.reset board components traces interior
  - hello.D11C.blink.reset.clock board components traces interior
      blink.c blink.make bootloader blink.ino video
  - hello.D11C.echo board components traces interior
      echo.ino video 
  - hello.D11C.serial.5V board components traces interior
  - hello.D11C.serial.3V3 board components traces interior
      serial.ino video

- ATSAMD11D
  - hello.D11D.echo board components traces interior
      openocd.cfg bootloader echo.ino video

- Interpreters
  - AVRSH
  - BASIC
  - FORTH
  - Espruino
  - MicroPython CircuitPython

- ESP8266
  - ESP-01
  - hello.ESP-01 board components traces holes interior
         echo.ino video
  - ESP-WROOM-02D
    - hello.ESP-WROOM-02D board components traces holes interior
         echo.ino video
         Python video

- ESP32
  - ESP32-WROOM-32
    - hello.ESP32-WROOM board components traces holes interior
         echo.ino video
         Python video

- Operating Systems
  - FreeRTOS
  - TinyOS
  - Mbed OS
  - ROS

- Systems
  - Rasberry Pi MATE
  - Beagle
  - Micro:bit

- debugging
  - hardware
    - inspect, reflow solder joints
    -  check component orientation, values
    -  verify data sheets
    -  confirm connector orientation
    -  measure supply voltages
    -  probe I/O signals
  - software
    - blink LED
    - add print statements
    - use embedded debugger
      - gdb, ddd
      - Atmel Studio

- assignment
  - individual assignment:
    - read a microcontroller data sheet
    - program your board to do something,
    - with as many different programming languages
         and programming environments as possible
  - group assignment:
    - compare the performance and development workflows
         for other architectures

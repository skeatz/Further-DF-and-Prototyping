## Embedded Programming

- architectures
  - von Neumann, Harvard
  - RISC, CISC
  - microprocessor, microcontroller
  - GPU, TPU
  - FPGA, TinyFPGA

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
  - 8051
  - PIC
  - MSP
  - AVR
    - ATtiny412 ATtiny45V
    - ATtiny1614 ATtiny44A
    - ATtiny3216
   - ARM
     - D11C D11D	
     - D21E
     - D51
   - Xtensa
     - ESP8266
     - ESP32
   - PSoC, xCORE, Propeller, Lattice, NVIDIA

- vendors
  - Octopart
  - Digi-Key
  - Mouser
  - RS Components
  - Element14
  - SparkFun
  - Adafruit

- packages
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
    - avrdude
    - hardware
      - header pads clip pins
      - Atmel-ICE
      - Arduino
      - ATmega16U2 Zaerc
      - FabtinyISP: Brian
  - UPDI (AVR 0,1-series)
    - software
      - pyupdi
           install: pip3 install intelhex pylint pyserial
           program: python3 pyupdi.py -d your_processor -c your_port -b your_baud_rate -f your_hex -v
      - hardware
        - hello.serial-UPDI.FT230X board components traces interior
        - hello.USB-UPDI.FT230X board components traces interior
  - JTAG (ARM)
    - software
      - OpenOCD
      - EDBG
           program: edbg -b -t target_type -pv -f binary_file
           read fuses: edbg -b -t target_type -F r,*,file_name
           write fuses: edbg -b -t target_type -F w,high_bit:low_bit,bit_value
    - hardware
      - Atmel-ICE
      - PICO
      - GoodFET
      - Raspberry Pi
      - Free-DAP
            hello.CMSIS-DAP.10.D11C board components traces interior
            hello.CMSIS-DAP.4.D11C board components traces interior
            hello.SWD.10-4 board components traces interior
               binary video
   - bootloader (all)

- assembly language
  - hex file
  - instruction set, opcodes
  - mnemonics, directives, expressions
  - avr-as
  - inline

- C
  - programming
  - GCC
    -  make files (tabs)
    -  bit operations
  - AVR
    - libc modules types math benchmarks
    - avr-libc binutils-avr gcc-avr
    - homebrew-avr
  - ARM
    - gcc-arm-none-eabi gdb-multiarch
    - homebrew-arm
  - Microchip
    - ASF
    - Studio
    - toolchains

- IDE
  - Atmel Studio
  - Arduino
  - Eclipse AVR
  - Firefly
  - Scratch
  - Modkit

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

- ATSAMD21E
   hello.D21E.echo board components traces interior
      bootloader echo.ino video

- ATSAMD51
   hello worlds

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

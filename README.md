 # CYFRAM
### Cypress F-RAM Master Library for Arduino

**F-RAMs** (*Ferroelectric RAMs*) are *nonvolatile RAMs* with very high endurance (exceeding 10^14 to 10^16 read/write cycles).

This library supports **I2C and SPI APIs** provided with the development kit *CY15FRAMKIT-001*. They where assembled as a lean all-in-one Arduino library to support generic Cypress F-RAM memories.

- The **I2C APIs** include initialization of block, write, current read and random read

- The **SPI APIs** include initialization of block, write/read memory, status register

Arduino standard libraries *Wire* and *SPI*  will be used for best MCU HW support.

Memory spefic functions like vendor-IDs, sleep, etc. and memory pins /W and /HOLD are not supported in this version. 


## Examples 

Two sketches within the *CY15FRAMKIT-001 Kit Setup* had been modified and analysed with a logic analyzer. 

- **FRAM_I2C_Example_2.ino:** This sketch was used to test **FM24W256, 256-Kbit (32K x 8) Serial (I2C) F-RAM**

- **FRAM_SPI_Example_2.ino:** This sketch was used to test **FM25W256, 256-Kbit (32K x 8) Serial (SPI) F-RAM**

All test results are part of this distribution and reside in the folders **logic** and **output**. 

Although other Cypress F-RAMs are not tested yet they should work until a size of 512-Kbit (64K x 8). Larger memories with 3 byte adress are not supported until yet. Grateful if you can send results of other tested memories. 

## More

- *Ferroelectric RAM:* https://en.wikipedia.org/wiki/Ferroelectric_RAM

- *nonvolatile RAMs (NVRAM):* https://en.wikipedia.org/wiki/Non-volatile_memory

- *CY15FRAMKIT-001:* 
http://www.cypress.com/documentation/development-kitsboards/cy15framkit-001-serial-f-ram-development-kit-guide

- *CY15FRAMKIT-001 Kit Setup (CY15FRAMKIT-001 Kit Setup - Kit Design Files,Documentation, Examples):*
http://www.cypress.com/file/278596/download

Links valid on 2017-08-27
 
<code> 
version=1.0.0
</code>

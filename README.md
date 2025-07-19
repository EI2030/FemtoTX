# Solar FemtoTX Landing Page for Project, Status & Updates

http://ei2030.github.io/FemtoTX

![logo](https://github.com/user-attachments/assets/e79211f1-7553-461b-b372-d3404e3b29ff)

7-18-2025
--

Current Milestone 3: Simulating Linux

Vedula is working on implementing the ZAP SoC on the FPGA Arty xc7a100tcsg324. A [Storm Core (ARM7)](https://github.com/freecores/storm_soc/blob/master/doc/STORM%20SoC%20-%20Datasheet%20and%20Implementation%20Guide.pdf) has been found to be completely implemented in an FPGA w/ Altera, therefore we may switch to that core, add EthMac, and  implement that one instead.  

6-17-2025
---

Vedula says:

1. I just created a tag, [solar_femtoTX_Milestone-1](https://github.com/srvedulageth/solar_femtoTx/releases/tag/solar_femtoTX_Milestone-1)

A very very basic EthMAC access test i put in.

1. SoC has ZAP core + EthMAC + UART(2 Instances) + Timer(2 Instances) + VIC(1 Instance)
2. Synthesized SoC for Xilinx xc7a100tcsg324-1.
3. Test bench is up with these modules. Ran few tests.
------------------------------------------------------

Synthesis performed on an [ARTY A7 (Artix-A7) 100T](https://digilent.com/shop/arty-a7-100t-artix-7-fpga-development-board
)

![image](https://github.com/user-attachments/assets/f6aa6043-2df5-43c0-ad59-5b62f0fc2c57)

6-06-2025 Update
--

The Ethernet controller will be using the [EthMac](https://github.com/freecores/ethmac) core 

The FemtoTX will be similar the ARM926EJ-based [SAM9x60](https://www.mouser.com/datasheet/2/268/SAM9X60_Data_Sheet_DS60001579-3443133.pdf) and [NU980](https://www.nuvoton.com/products/iot-solution/iot-platform/numaker-rtu-nuc980/?_gl=1*ouv4oz*_ga*NjY1NTAwNzM0LjE3NDkyMzcxODc.*_ga_6JZ62QPH6N*czE3NDkyMzcxODUkbzEkZzEkdDE3NDkyMzg5NjkkajYwJGwwJGgw) boards by Microchip and Nuvoton

https://github.com/EI2030/Low-power-E-Paper-OS/blob/master/Hyperlinks.md#arm9-armv5-socs

06-02-2025
--

Vedula has completed synthesis of a ZAP processor on an Artix A7!:

[Github repository
](https://github.com/srvedulageth/solar_femtoTx)

Vedula's notes:

"Please see Save/ dir for Synthesis report.

Added a separate Readme for convenience."

https://github.com/srvedulageth/solar_femtoTx/blob/main/README.solar_femtoTx 



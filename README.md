# Solar FemtoTX Landing Page for Project, Status & Updates

http://ei2030.github.io/FemtoTX

![logo](https://github.com/user-attachments/assets/e79211f1-7553-461b-b372-d3404e3b29ff)

8-24-25
--
<img width="959" height="93" alt="image" src="https://github.com/user-attachments/assets/a7f9cce9-b584-4fd9-99a4-c2c721b2497e" />

<img width="961" height="1843" alt="image" src="https://github.com/user-attachments/assets/5e724366-9dce-4f93-8a17-084d973445e6" />

https://en.wikipedia.org/wiki/Transistor_count#Microprocessors



8-13-25
--

Vedula has completed [synthesis](https://github.com/srvedulageth/solar_femtoTx/tree/solar_femtoTX_ms2/src) and loading of the FPGA with UART & ZAP Core. He made an LED test, which shows 3 continuously lit LEDs, and one blinking. He connected UART Tx (output from ZAP SoC), and whenever he presses a key, the LED comes back as it was connected to tx_0, which is the blinking LED.

https://github.com/user-attachments/assets/a891d421-b59e-4ba2-997c-f307857429f3


This step was an intermediate stage before he can begin booting linux, which he will work on next. 

7-22-25
--

https://www.allaboutcircuits.com/ip-cores/all/P720/ Other ISAs that may be of use/complement ZAP core

https://github.com/stnolting/neorv32 

https://www.allaboutcircuits.com/ip-cores/processor/

https://www.allaboutcircuits.com/ip-cores/processor/arm4u/  https://github.com/freecores/arm4u

https://www.allaboutcircuits.com/ip-cores/processor/aor3000/ https://github.com/alfikpl/aoR3000

https://www.allaboutcircuits.com/ip-cores/processor/mips-enhanced/ 

https://opencores.org/projects/mips789

https://github.com/freecores/mips789/tree/master/core



7-21-25
--

<img width="583" height="191" alt="ARM cores" src="https://github.com/user-attachments/assets/24c99442-2df0-4b88-bae4-fa8eb4cefcbf" />

<img width="464" height="211" alt="SVP" src="https://github.com/user-attachments/assets/d4c27619-f312-4620-85ca-20b2570e4b6b" />

<img width="481" height="142" alt="corelang" src="https://github.com/user-attachments/assets/1e151bc2-f64b-4668-8668-0ca9c74ffa59" />

See [paper](https://github.com/EI2030/FemtoTX/blob/gh-pages/ARM%20compatible%20core%20paper.pdf) for background and candidate cores.

FA526: https://www.innopower-tech.com/html/products/functional/FA5.jsp

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



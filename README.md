# Solar FemtoTX Landing Page for Project, Status & Updates

http://ei2030.github.io/FemtoTX

![logo](https://github.com/user-attachments/assets/e79211f1-7553-461b-b372-d3404e3b29ff)


11-26-2025
--

Vedula has reported pings work, while timeouts occur. As of 12-3, he is currently debugging. 

![IMG_2649](https://github.com/user-attachments/assets/65e57f84-c8b2-4f90-826b-44b6933a477c)


11-05-2025
--

Vedula has completed TX and RX continuous testing!

![WhatsApp Image 2025-11-05 at 11 00 50 AM](https://github.com/user-attachments/assets/539316e9-e3c2-46cd-8ed2-8a8dd81f1334)

https://github.com/user-attachments/assets/7d4f2f48-4a5c-43dc-9d0d-9d9809e34246

https://youtu.be/E1b18wrB_ZA 

Next up: validation on FPGA of full duplex.

10-25-2025
--

Vedula has completed EthMac Tx. He sent data from the ZAP SoC to his Windows desktop and captured the Tx using Wireshark. He will test Rx now and then work on booting linux.

![WhatsApp Image 2025-10-24 at 4 00 12 PM](https://github.com/user-attachments/assets/2a87f70f-0524-4bfa-b7f0-e1fddcb6d0fd)

9-6-25
--

VS reports:
1. Checked in code with EthMAC integrated.
2. Implemented SoC with Ethmac. No errors and able to transfer on uart.
3. Next Task
    Write Driver for EthMAC. 

8-24-25
--
the [ZAP core](https://github.com/krevanth/ZAP?tab=readme-ov-file#1-introduction) has cache:

<img width="902" height="451" alt="image" src="https://github.com/user-attachments/assets/b0ad6ef5-db45-4c04-809b-cc24eb7f7f1a" />

<img width="959" height="93" alt="image" src="https://github.com/user-attachments/assets/a7f9cce9-b584-4fd9-99a4-c2c721b2497e" />

<img width="961" height="1843" alt="image" src="https://github.com/user-attachments/assets/5e724366-9dce-4f93-8a17-084d973445e6" />

https://en.wikipedia.org/wiki/Transistor_count#Microprocessors

https://www.techrxiv.org/users/814616/articles/1270555-a-heuristic-method-for-designing-solar-circuits
Estimating the power consumption can be tricky. At 130nm, 22nm, and 3nm. The budget of this project will allow 130nm, but it's unclear how much funding would be [needed](https://private-user-images.githubusercontent.com/76194453/472805826-5832b85e-3557-4ee9-b29a-1bd89633fc49.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTYwNTIxMDksIm5iZiI6MTc1NjA1MTgwOSwicGF0aCI6Ii83NjE5NDQ1My80NzI4MDU4MjYtNTgzMmI4NWUtMzU1Ny00ZWU5LWIyOWEtMWJkODk2MzNmYzQ5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MjQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODI0VDE2MTAwOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWI4ZGU1ZGYxMjM1M2VhMTRhNzFhNjMzYTU4NWJmNzQ1ZjUzMGUzOWY4MDMwNDA2ZjU1ZjNlODg2YWNlZjcwZmQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.9WhTfnsIz_mWtFRyQu0CIaWyyPlV3ahqx-uBLqk2uCU) for [22nm](https://www.linkedin.com/posts/ali-kamaly_semiconductors-chipdesign-validation-activity-7355930371999383553-wzxl/), and eDRAM

https://www.musesemi.com/full-block-tapeout-pricing
https://www.cmc.ca/globalfoundries-22fdx-fdsoi-22-nm/ 
https://www.src.org/calendar/e003676/barth.pdf

<img width="386" height="172" alt="image" src="https://github.com/user-attachments/assets/625813ba-012e-49e3-8062-72cfbdc2fe55" />


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



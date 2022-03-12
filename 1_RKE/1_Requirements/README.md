
# Introduction
Remote Key Entry is an electronic lock that controls access to a building or vehicle without using a conventional mechanical key. The term Remote Key entry system literally means controlled some functionality of car by a remote such as lock, unlock, alarm activation and approch light at or near the car, which requires entering a default (or self-programmed) numeric code. RKE transmission requires two components - a transmitter and a receiver. Transmitter - RKE key fob, other ID device with RKE integrated Receiver - Body Control ECU, other ECU with integrated RKE. RKE operates by broadcasting radio waves on a particular frequency unidirectionally. RKE systems implement encryption and rolling code algorithms to prevent car thieves from intercepting and spoofing the telegrams. 

------------------------
# danesh 

<h1 align="center"> RKE </h1>
<i><h3 align = "center"> Remote Keyless Entry</h3></i>
<h3 align = "center"> Remote keyless entry (RKE) system is a system designed to remotely lock or unlock access to automobiles.  </h3>


## PRODUCT RESEARCH
<p align="center">
  <img width="1080 "height="342 " src="https://github.com/shri-vaishnavi/M3_Group55/blob/main/1_RKE/Images/RSK.png ">
</p>
<br>
<h5><j>The Remote Keyless System refers to a lock that uses an electronic remote control to access functions such as lock, unlock, alarm activation etc. Keyless remotes contain a short-range radio transmitter, and works within a certain range of the car to work. Remote Keyless System has a transmitter and a receiver to communicate. Receiver is the Body Control ECU, another ECU with integrated RKE Transmitter in the target vehicle. RKE Transmitter is incorporated with RKE key fob and other ID device which works by sending radio waves in a single direction on a certain frequency.When a button is pushed, it sends a coded signal by radio waves to a receiver unit in the car, which performs the functions accordingly. The functions of a remote keyless entry system are contained on a key fob. The RKE systems use encryption and rolling code techniques to prevent intercepting of command signals from the key. The rolling code is a pseudo random number generator generated differently for each time. Here we have discussed RKE system implimented in the car.
In this project we will use STM32F407 to emulate these functionalities. 
</j></h5>

# danesh


## FEATURES #
The project is all about programming the RKE to impliment its below mentioned functions. The features implimneted differs or a part of the real time RKE system. 
1. RKE transmission requires two components - a transmitter and a receiver. Communication takes place in uni-direction. 
* Transmitter - RKE key fob, other ID device with RKE integrated 
* Receiver - Body Control ECU, other ECU with integrated RKE 
2. RKE operates by broadcasting radio waves on a particular frequency unidirectionally. 
3. RKE systems implement encryption and rolling code algorithms are used to prevent car from being intercepted and spoofed. 
4. RKE functions implimented are: <br>

| Input command              |                       Output                                                   |
| ---------------------------| -------------------------------------------------------------------------------|
| Blue switch pressed once   |  1. All led on at the same time. <br> 2.  Print lock.                          |
| Blue switch pressed twice  | 1. All led off at the same time. <br> 2.  Print unlock.                        |
| Blue switch pressed thrice |  1. All led on in clockwise manner <br> 2. Print alarm activation/deactivation |
| Blue switch pressed for four times | 1. All led on in anti-clockwise manner <br> 2. Print approach light   |
	
-------------------------------------------------------------------------------------------------------------------
#
#
# SWOT Analysis
![Simple-Matrix-SWOT-Template_Nov2020](https://user-images.githubusercontent.com/98829237/157732602-74318b52-e360-4451-a536-ddfc67f7e57e.jpg)

-----------------------

##  4W's & 1H
1) what ?
  * Wireless key for the smart cars.
2) who ?
  * The people who wants to control their car wirelessely.
3) when ?
  *  User want to locking and unlocking, alarm function activation.
4) where ?
  * Outside/Inside and near the car or at a frequent range.
5) how ?
  * By pressing the blue button in the remotr key.
----------------------

# Requirements

##  High Level Requirements
 
|ID| Description|
|----|----|
|HLR1|It shall be lock when the blue switch press one time|
|HLR2|It shall be unlock when the blue switch press two times|
|HLR3|It shall be alaram activation/decactivation when the blue switch press two three|
|HLR4|It shall be approach when the blue switch press two four|

## Low Level Requirements

|ID| Description|
|----|----|
|HLR1_LLR1|All LED's are ON at the same time|
|HLR2_LLR2|All LED's are OFF at the same time|
|HLR3_LLR3|All LED's are ON in Clockwise-direction|
|HLR4_LLR4|All LED's are ON in Anti-Clockwise-direction|

-------------------------------------------

# MATERIALS REQUIRED 
 
 
* Power supply 1.2v regulator POR/PDR/PVD

2. Analog and Digital  
* 2-Channel 2x 12-bit DAC
* Temperature sensor

3. Control
* 10x 16-bit timer
* 2x 16-bit motor control PWM synchronized AC timer
* 2x 32-bit timer
       
##  4. Communication protocal

       * Camera interface
       * 3x SPI,2x i^2S,3xi^2C
       * Etherent MAC 10/100 with IEEE 1588
       * 2x CAN 2.0B
       * 1x USB 2.0 OTG FS/HS
       * 1X USB 2.0 OTG FS
       * 6X USART LIN,smartcard,IrDA,modem control
       
##   5. Memory 

        * Up to 1-Mbyte Flash memory
       * Up to 192-Kbyte SRAM
       * 80-byte + 4-Kbyte backup SRAM
   * Flash memory of up to 1 megabyte
  * Compact Flash, SRAM, PSRAM, NOR, and NAND memories are all supported by this versatile static memory controller.

4. Low-wattage operation
* Modes of sleep, stop, and standby
* RTC power supply, 2032 bit backup registers, and an optional 4 KB backup SRAM

5. Mode of debugging
   * Cortex-M4 Embedded Trace MacrocellTM
   * Interfaces for serial wire debug (SWD) and JTAG
 
6. With interrupt capabilities, up to 140 I/O ports are available.
   * Up to 136 high-speed I/Os at 84 MHz
   * I/Os with a V tolerance of up to 138 5
   
7. There are up to 15 communication interfaces available.
   * Up to three I2C interfaces (SMBus/PMBus) are available.
   * Up to four USARTs and two UARTs (10.5 Mbit/s, ISO 7816 interface, LIN, IrDA, and modem control) are available.
   * To achieve audio class precision via internal audio PLL or external clock, there are up to three SPIs (42 Mbits/s), two of which are muxed full-duplex I2S.
   * 2 CAN (Controller Area Network) interfaces (2.0B Active)
   * SDIO (Serial Digital Interface) 
   
8. Advanced interconnection
   * Full-speed USB 2.0 device, host, and OTG controller with on-chip PHY
   * High-speed/full-speed USB 2.0 device/host/OTG controller with dedicated DMA, full-speed PHY on-chip, and ULPI
   * Supports IEEE 1588v2 hardware, MII/RMII, and 10/100 Ethernet MAC with dedicated DMA.   
  
-----------------------------------------------------------



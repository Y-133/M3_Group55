# Table of content :
1. Product research 
2. Features
   * Problem solving approach:
3. 4W 1H
4. SWOT analysis  
5. Materials req (STM327407)
6. Requirements:
	  * HLR
  	* LLR
--------------------------
<h1 align="center"> BiCom </h1>
<h3 align = "center"> BiCom System designed to remotely lock or unlock to access some features of.  </h3>

## Introduction
  * Bi-com system ,is a system that's designed to remotely lock or unlock the automobiles, RKE operates by broadcasting radio waves on a selected frequency unidirectionally,RKE      systems implement encryption algorithms to stop car thieves from intercepting and spoofing the telegram.
  * The term bi-com, is additionally called keyless entry or remote central locking, refers to a lock that uses an electronic remote as a key which is activated by a handheld       device or automatically by proximity.
  * Widely employed in automobiles, an RKS performs the functions of a regular car key without physical contact. When within some yards of the car, pressing a button on the         remote can lock or unlock the doors, and should perform other functions.
## PRODUCT RESEARCH
<p align="center">
  <img width="1080 "height="342 " src="https://github.com/shri-vaishnavi/M3_Group55/blob/main/1_RKE/Images/RSK.png ">
</p>
<br>
<p align = "justify"> The Remote Keyless System refers to a lock that uses an electronic remote control to access functions such as lock, unlock, alarm activation etc. Keyless remotes contain a short-range radio transmitter, and works within a certain range of the car to work. Remote Keyless System has a transmitter and a receiver to communicate. Receiver is the Body Control ECU, another ECU with integrated RKE Transmitter in the target vehicle. RKE Transmitter is incorporated with RKE key fob and other ID device which works by sending radio waves in a single direction on a certain frequency.When a button is pushed, it sends a coded signal by radio waves to a receiver unit in the car, which performs the functions accordingly. The functions of a remote keyless entry system are contained on a key fob. The RKE systems use encryption and rolling code techniques to prevent intercepting of command signals from the key. The rolling code is a pseudo random number generator generated differently for each time. Here we have discussed RKE system implimented in the car.
In this project we will use STM32F407 to emulate these functionalities. 
</p>
## FEATURES #

The project is all about programming the Biocom to impliment its below mentioned functions. The features implimneted differs or a part of the real time biocom system. 
1. Biocom transmission requires two components - a transmitter and a receiver. Communication takes place in bi-direction. 
* Transmitter - The info transmitted to the keyfob,
* Receiver - Body Control ECU, other ECU with integrated biocom system,send back to the keyfob to display the status.  
2. The term bi-com, is also called keyless entry or remote central locking, refers to a lock that uses an electronic remote control as a key which is activated by a handheld         device or automatically by proximity.
3. Widely used in automobiles, an RKS performs the functions of a standard car key without physical contact. When within a few yards of the car, pressing a button on the remote    can lock or unlock the doors, and may perform other functions.

| Input command              |                       Output                                                    |
| ---------------------------| ------------------------------------------------------------------------------- |
| Blue switch pressed once   |  1. All led on at the same time. <br> 2.  Print windows status.                 |
| Blue switch pressed twice  | 1. All led off at the same time. <br> 2.  Print alram status.                   |
| Blue switch pressed thrice |  1. All led on in clockwise manner <br> 2. Print car battery info status        |
| Blue switch pressed for four times | 1. All led on in anti-clockwise manner <br> 2. Print Door status        |

### PROBLEM SOLVING APPROACH
The main function used to check the condition. The button pin is pulled up and the pin is monitored continuosly for change using the STM32F407 controller. When the switch press event is identified the countis incremented and coressponding function is done.

--------------------------------------




----------------------
##  4W's & 1H
| Sl.No | Questions | Description | 
| :-----: | :-----: | ----- |
| 1. | What | Wireless key for the smart cars. In this project we will impliment RKE functionalities as said above. |
| 2. | Who |Any car user who wants to control the car function from a certain range. | 
| 3. | When |User wants to lock or unlock or when using other functions. |
| 4. | Where |The features can be accessed using the remote key from inside or from certain range. | 
| 5. | How |By pressing the button in the remote key. Here we will use blue button on the STM32F407 to emulate these functionalities. |
#
#
# SWOT Analysis
![Simple-Matrix-SWOT-Template_Nov2020](https://user-images.githubusercontent.com/98829237/157732602-74318b52-e360-4451-a536-ddfc67f7e57e.jpg)
----------------------

# MATERIALS REQUIRED 

 STM32F407 is only board required for this project. Its technical speficication is given below.
 | Sl. No |  Title | Description |
 | ------- | ------- | -----------|
 | 1. | Power supply | 1.8 V - 3.6 V |
 | 2. |Analog and Digital  | 2-Channel 2x 12-bit DAC <br> Temperature sensor |
 | 3. | Control | 1. 10x 16-bit timer <br>2. 2x 16-bit motor control PWM synchronized AC timer <br>3. 2x 32-bit timer |
 | 4. | Peripherals | 1. Camera interface <br>2. 3x SPI,2x i^2S,3xi^2C<br>3. Etherent MAC 10/100 with IEEE 1588 <br> 4. 2x CAN 2.0B <<br> 5. 1x USB 2.0 OTG FS/HS <br>6. 1X USB 2.0 <br>7. OTG FS <br>8. 6X USART LIN,smartcard,IrDA,modem control   
| 5. |Memory | 1. Up to 1-Mbyte Flash memory <br> 2. Up to 192-Kbyte SRAM <br>3.  80-byte + 4-Kbyte backup SRAM <br>4. Flash memory of up to 1 megabyte <br>5.  Compact Flash, SRAM, PSRAM, NOR, and NAND memories are all supported by this versatile static memory controller. |
| 6. | Low-wattage operation | 1. Modes of sleep, stop, and standby <br> 2. RTC power supply, 2032 bit backup registers, and an optional 4 KB backup SRAM |
| 7. | Mode of debugging | 1. Cortex-M4 Embedded Trace MacrocellTM <br>2.Interfaces for serial wire debug (SWD) and JTAG |
| 8. | Communication interfaces | 1. Up to three I2C interfaces (SMBus/PMBus) are available. <br> 2. Up to four USARTs and two UARTs (10.5 Mbit/s, ISO 7816 interface, LIN, IrDA, and modem control) are available. <br> 3. To achieve audio class precision via internal audio PLL or external clock, there are up to three SPIs (42 Mbits/s), two of which are muxed full-duplex I2S. <br> 4. 2 CAN (Controller Area Network) interfaces (2.0B Active) <br>5. SDIO (Serial Digital Interface)  |   
| 9. |Advanced interconnection | 1. Full-speed USB 2.0 device, host, and OTG controller with on-chip PHY <br> 2. High-speed/full-speed USB 2.0 device/host/OTG controller with dedicated DMA, full-speed PHY on-chip, and ULPI <br> 3. Supports IEEE 1588v2 hardware, MII/RMII, and 10/100 Ethernet MAC with dedicated DMA. <br> |
-----------------------------------
# Requirements

## HIGH LEVEL REQUIREMENTS
HLR     | DESCRIPTION
--------|-----------------------
HLR_1   |It should able to check the window status.
HLR_2   |It should able to check the alram status.
HLR_3   |It should able to check car battery info status.
HLR_4   |It should able to check Door status.

## LOW LEVEL REQUIREMENTS:- ##
| HLR_ID |LLR_ID | Design_consideration | 
| :-----: | :-----: | -------------------- | 
| HLR_1 | LLR_1.1 | Controller checks for any change in the pin state connected to the button continuously |
| | LLR_1.2 | If state change to '1' increment count |  
| | LLR_1.3 | Check count condition| 
| | LLR_1.4 | If count is equal to one, Turn on all LED at the same time for 5 seconds| 
| HLR_2 | LLR_2.1 | Controller checks for any change in the pin state connected to the button continuously|
| | LLR_2.2 | If any change increment count | 
| | LLR_2.3 | Check count condition| 
| | LLR_2.4 | If count is equal to two, Turn off all LED at the same time for 5seconds |
| HLR_3 | LLR_3.1 | Controller checks for any change in the pin state connected to the button continuously |
| | LLR_3.2 | If any change increment count |  
| | LLR_3.3 | Check count condition| 
| | LLR_3.4 | If count is equal to three, Turn on all LED clock wise for 5 seconds| 
| HLR_4 | LLR_4.1 | Controller checks for any change in the pin state connected to the button continuously|
| | LLR_4.2 | If any change increment count |  
| | LLR_4.3 | Check count condition| 
| | LLR_4.4 | If count is equal to four, Turn on all LED counter clock wise for5 seconds| 

------------------------------





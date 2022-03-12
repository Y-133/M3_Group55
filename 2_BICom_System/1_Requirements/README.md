## FEATURES #

The project is all about programming the Biocom to impliment its below mentioned functions. The features implimneted differs or a part of the real time biocom system. 
1. Biocom transmission requires two components - a transmitter and a receiver. Communication takes place in bi-direction. 
* Transmitter - The info transmitted to the keyfob,
* Receiver - Body Control ECU, other ECU with integrated biocom system,send back to the keyfob to display the status.  
2. The term bi-com, is also called keyless entry or remote central locking, refers to a lock that uses an electronic remote control as a key which is activated by a handheld         device or automatically by proximity.
3. Widely used in automobiles, an RKS performs the functions of a standard car key without physical contact. When within a few yards of the car, pressing a button on the remote    can lock or unlock the doors, and may perform other functions.

| Input command              |                       Output                                                   |
| ---------------------------| -------------------------------------------------------------------------------|
| Blue switch pressed once   |  1. All led on at the same time. <br> 2.  Print windows status.              |
| Blue switch pressed twice  | 1. All led off at the same time. <br> 2.  Print alram status.              |
| Blue switch pressed thrice |  1. All led on in clockwise manner <br> 2. Print car battery info status |
| Blue switch pressed for four times | 1. All led on in anti-clockwise manner <br> 2. Print Door status   |

--------------------------------------













#  4W's & 1H

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

## HIGH LEVEL REQUIREMENTS
HLR     | DESCRIPTION
--------|-----------------------
HLR_1   |It should able to check the window status.
HLR_2   |It should able to check the alram status.
HLR_3   |It should able to check car battery info status.
HLR_4   |It should able to check Door status.

## LOW LEVEL REQUIREMENTS
LLR     | DESCRIPTION
--------|-----------------------
LLR_1   |It should display the status of lock the device.
LLR_2   |It should display the status of unlock the device.
LLR_3   |It should display the alarm ON status.
LLR_4   |It should display the alarm OFF status.

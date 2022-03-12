
# 1.1 HIGH LEVEL TEST PLAN

| Test ID | Description | Input | Expected output | Actual Output | 
| --- | --- | --- | --- | --- | 
| 01 | Lock the car | Press the button once | Display Car Window status | Displayed Car Window status  | 
| 02 | Car Unlock | Press the button twice |  Display Car alarm status  | Displayed Car alarm status  | 
| 03 | Alarm activation and deactivation | Press the button thrice | Display Car Battery Status | Displayed Car Battery Status | 
| 04 | Approach light | Press the button four times | Display Car Door Status | Displayed Car Door Status | 

### Here below are the some of the *unity test/ unity framework* test plans there are so many but I have only mentiones some of the test cases here.

# 1.2 LOW LEVEL TEST PLAN

| Test ID | Description | Input | Expected output | Actual Output | Passed Or Not |
| --- | --- | --- | --- | --- | --- |

| Test ID (for LED)| Description | Input | Expected output | Actual Output | passed/not |
| --- | --- | --- | --- | --- | --- |
| 01 | All LED on | 1 User Button Press | All LEDs ON |All LEDs ON | ✅ |
| 02 | All LED off| 2 User Button Presses | All LEDs OFF | All LEDs OFF | ✅ |
| 03 | LED ON Clockwise | 3 User Button Presses | LED ON Clockwise Rotation | LED ON Clockwise Rotation | ✅ | 
| 04 | LED ON anti-clockwise | 4 User Button Presses |LED ON Anticlockwise Rotation | LED ON Anticlockwise Rotation | ✅ |

| Test ID (for Button Count)| Description | Input | Expected output | Actual Output | passed/not |
| --- | --- | --- | --- | --- | --- |
| 01 | Button count | Press the button once | 1 and print locked| 1 and print locked| ✅ |
| 02 | Button count | Press the button twice | 2  and print unlocked| 2 and print unlocked| ✅ |
| 03 | Button Count | Press the button thrice | 3 and print alaram ON| 3 and print alaram ON| ✅ |
| 04 | Button Count | Press the button four times | 4 and print alaram OFF| 4 nd print alaram OFF| ✅ |

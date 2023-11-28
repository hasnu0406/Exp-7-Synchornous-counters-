# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/
### UPCOUNTER:
![Screenshot 2023-11-28 204919](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/b5fd7566-7850-4847-8601-77da5b3ea60b)

### DOWNCOUNTER:
![Screenshot 2023-11-28 205011](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/b786decc-4fb9-4ac2-99a1-05ec8aead719)


### RTL LOGIC UP COUNTER AND DOWN COUNTER  
### UPCOUNTER:
![UPCOUNTER-DIAGRAM](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/46336570-d6bb-47d0-97e9-607101ed8cf9)

### DOWNCOUNTER:
![DOWNCOUNTER-DIAGRAM](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/f72ae682-593a-4b59-9a91-728102e158ec)


### TIMING DIAGRAMS FOR COUNTER 
### UPCOUNTER:
![UPCOUNTER-WAVEFORM](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/f6e6ea5e-dfaf-4d72-8990-68b9ec8f3b60)

### DOWNCOUNTER:
![DOWNCOUNTER-WAVEFORM](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/9519347f-5979-4466-9a22-b50ccf592667)


### TRUTH TABLE 
### UPCOUNTER:
![UPCOUNTER-TRUTH TABLE](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/be1a0827-4571-4bf3-b3da-d718f579bbe7)

### DOWNCOUNTER:
![DOWNCOUNTER-TRUTH TABLE](https://github.com/hasnu0406/Exp-7-Synchornous-counters-/assets/135305537/3e195414-f879-40d5-9e71-2861f6d35d80)

### RESULTS 

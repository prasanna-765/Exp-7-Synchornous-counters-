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

1.Create a new project in QuartusII software.

2.Name the project as uc for upcounter and dc for
down counter. 

3.Create a new verilog hdl file in the project file. 

4.Name the module as dc and uc for
down counter and up counter. 

5.Within the module declare input and output variables. 

6.Create a loop using if-else with condition parameter as reset value. 

7.End the loop. 

8.End the module



### PROGRAM 

Program for flipflops  and verify its truth table in quartus using Verilog programming.

Developed by: Prasanna A 

RegisterNumber:  23005675

UP COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/34034b79-0e1b-4771-921e-46b3e14d3ea4)

DOWN COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/00cf6c88-c050-407f-9eba-195789e3914b)


### RTL LOGIC UP COUNTER AND DOWN COUNTER  

UP COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/165ce2a5-33fb-418c-9fb3-7530afb9be5a)

DOWN COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/9045a597-6378-4395-9dfb-1802364fcacd)

### TIMING DIGRAMS FOR COUNTER  

UP COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/9456765d-2bbc-4bc3-b55b-4f0a14089b4d)

DOWN COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/81ecf3a5-868d-453a-aae9-b4b03b95e7de)

### TRUTH TABLE 

UP COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/01b8043b-6eac-4744-bb0d-0bf8e082e57d)

DOWN COUNTER:

![image](https://github.com/prasanna-765/Exp-7-Synchornous-counters-/assets/150009505/1377c8f1-1893-435f-b38f-bf4459316826)

### RESULTS 

Thus Synchornous counters up counter and down counter circuit are studied and the truth table for
different logic gates are verified

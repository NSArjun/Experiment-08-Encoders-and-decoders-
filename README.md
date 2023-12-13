# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure
Step 1: Create module encoder and decoder.
Step 2: Get inputs and outputs for encoders and decoders.
Step 3: Perform "or" operation for encoder and "and" logic for decoders.
Step 4: Perform RTL LOGIC and get waveform.
Step-5: End the module.



### PROGRAM 

Program for Endocers and Decoders  and verify its truth table in quartus using Verilog programming.
Developed by: ARJUN N S
RegisterNumber:  212223230020

## CODE:
### ENCODER:
![ENCODER CODE](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/5fb9f3a2-6545-49f5-9a3b-c7553355a892)

### DECODER:
![DECODER CODE](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/a5eb8b20-8d5e-472b-b4b6-917cea6a1ed1)

## RTL LOGIC: 
### ENCODER:
![ENCODER LOGIC](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/db1ad411-9b99-42b9-9ff4-1b6e0553b5c0)

### DECODER:
![DECODER LOGIC](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/c4d9b72b-9572-4fc5-84e6-08a7dec5158e)

## TIMING DIGRAMS  
### ENCODER:
![ENCODER TIME](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/1cc9e5db-e8d3-457c-a08b-cf1d20615086)

### DECODER:
![DECODER TIME](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/d459b455-3eec-494d-af98-0efcaa278512)

## TRUTH TABLE 
### ENCODER:
![ENCODER TT](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/101df939-83cd-455b-86e4-6da9a007a407)

### DECODER:
![DECODER T](https://github.com/NSArjun/Experiment-08-Encoders-and-decoders-/assets/148233801/68a38638-86f3-4761-abbd-87d8323c000e)

### RESULTS:
Thus the program to desing encoder and decoder is done.

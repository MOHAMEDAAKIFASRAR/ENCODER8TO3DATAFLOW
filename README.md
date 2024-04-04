## NAME:MOHAMEDAAKIFASRAR S
## REG NO:212223240088
### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**
~~~
STEP-1 Define Inputs and Outputs

STEP-2 Understand the Encoder Functionality

STEP-3 Design the Functional Table

STEP-4 Write Verilog Code

STEP-5 Verify Verilog Code

STEP-6 Synthesize the Design

STEP-7 Implement in FPGA

STEP-8 Verify Functionality on FPGA
~~~

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:212223240088
*/
~~~
module Exp_05(a0, a1,a2, d0,d1,d
input d0,d1, d2, d3,d4, d5, d6,d7;
output a0, a1,a2;
assign a0=d1 | d3|d5|d7;
assign a1=d2|d3|d6| d7 ;
assign a2=d4 | d5 | d6 | d7 ;
endmodule
~~~

**RTL LOGIC FOR ENCODER 8 TO 3 IN DATAFLOW MODELLING**:
![RTL 2](https://github.com/MOHAMEDAAKIFASRAR/ENCODER8TO3DATAFLOW/assets/148514683/9963757a-6250-453a-9ee6-4722713b2349)


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![TIMEFLOW2](https://github.com/MOHAMEDAAKIFASRAR/ENCODER8TO3DATAFLOW/assets/148514683/c07d813e-fcc7-4372-be14-3988f8b4faaa)


**RESULTS**
Thus the given experiment was completed successfully.





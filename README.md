### ENCODER 8TO3 DATAFLOW Modelling
## NAME: DEEPAK JG
## REG NO: 24901065
## EXP NO:3 ENCODER 8TO3 DATAFLOW MODELLING


## AIM:

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

## SOFTWARE REQUIRED:
Quartus prime

## THEORY:

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

## TRUTH TABLE:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

1. Type the program in Quartus software.
 2. Compile and run the program.
 3. Generate the RTL schematic and save the logic diagram.
 4. Create nodes for inputs and outputs to generate the timing diagram.
 5. For different input combinations generate the timing diagram

**PROGRAM**
~~~
module Encoder(A2,A1,A0,y0,y1,y2,y3,y4,y5,y6,y7);
input y0,y1,y2,y3,y4,y5,y6,y7;
output A2,A1,A0;
assign A2 = ( y4 | y5 | y6 | y7);
assign A1 = ( y2 | y3 | y6 | y7);
assign A0 = ( y1 | y3 | y5 | y7);
endmodule
~~~

## RTL OUTPUT:
![Screenshot 2024-11-27 184156](https://github.com/user-attachments/assets/26013712-d99c-43c7-b491-a0bb0e7a0139)


## OUTPUT WAVEFORM:
![Screenshot 2024-11-27 185254](https://github.com/user-attachments/assets/143f0791-e76c-487a-a560-0e880a42b858)

## RESULT:
Thus Encoder 8 to 3 in Dataflow modelling is implemented successfully using verilog software.





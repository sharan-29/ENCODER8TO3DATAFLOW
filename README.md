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

1.Type the program in Quartus software

2.Compile and run the program

3.Generate the RTL schematic and save the logic diagram

4.Create nodes for inputs and outputs to generate the timing diagram

5.For difference input combination generate the timing diagram

**PROGRAM**
```
module exp5(bin,A0,A1,A2);
input [0:7] bin;
output A0,A1,A2;

assign A0=(bin[4]|bin[5]|bin[6]|bin[7]);

assign A1=(bin[2]|bin[3]|bin[6]|bin[7]);
assign A2=(bin[1]|bin[3]|bin[5]|bin[7]);
endmodule
```

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:212224230260
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![image](https://github.com/user-attachments/assets/e2d93f90-564c-4ced-955e-84dcfed7c4dd)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![exp 5](https://github.com/user-attachments/assets/5bf0933d-863c-4ed7-8e0a-9d5601768da4)


**RESULTS**

The program to encode 8 : 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables are verified





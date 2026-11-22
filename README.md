# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

~~~
module boolean_function (
    input A, B, C, D,
    output F
);

assign F = (~A & ~B & ~C & ~D) |
           ( A & ~C & ~D )     |
           (~B &  C & ~D )     |
           (~A &  B &  C &  D) |
           ( B & ~C &  D );

Endmodule

~~~

Developed by: N.Surya

Register Number: 212225040442


**Timing Diagram**

<img width="1920" height="1080" alt="Screenshot 2026-10-23 105913" src="https://github.com/user-attachments/assets/5603b90c-cc04-412b-96f7-cbc364d12ada" />

**RTL realization**

<img width="1920" height="1080" alt="Screenshot 2026-10-23 105714" src="https://github.com/user-attachments/assets/9af3d42c-0620-4f1f-93b4-ce612ccc39c2" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


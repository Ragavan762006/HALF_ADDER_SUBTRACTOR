# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![399066333-b0e13ed2-1f1b-4b46-82ee-ecdd5f99bcaf](https://github.com/user-attachments/assets/f32c53bb-c674-4f62-8d10-6821280c09b2)
**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
i)HALF ADDER
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry

i)HALF SUBTRACTOR
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule

```
**RTL Schematic**
**Half Adder**:
![399079551-919fa1d7-ce17-4e04-b9d5-5d1221a1f06f](https://github.com/user-attachments/assets/65954346-44c5-4ec4-a97f-5c2e72f3222d)
**Half Subtractor**:
![399079576-1deb8ffb-6f40-4fa8-be6e-6eaf1939297c](https://github.com/user-attachments/assets/c49323f0-8af4-4159-9aa2-cef486d0c309)

**Output/TIMING Waveform**
**Half Adder**:
![399079600-e8554643-3e02-43ae-88df-767aacced0f4](https://github.com/user-attachments/assets/2e43ba95-55c2-43f7-80c9-8525265fe64c)
**Half Subtract**:
![399079623-0df76d69-7083-4447-a3ce-ee30e6a4dac6](https://github.com/user-attachments/assets/0db6b858-b105-4042-9bf3-32d713b71cb7)
**Result:**
Thus the OUTPUT's of Encoder and Decoder are verified by synthesizing and simulating the VERILOG code.

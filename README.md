**EXP3: HALF ADDER AND SUBTRACTOR**

NAME: ARJUN.K

REFERENCE NO: 24900977

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

HALF ADDER

![image](https://github.com/user-attachments/assets/49e712fd-ac53-4e6c-9a61-d1128dac1007)


HALF SUBRACTOR

![image](https://github.com/user-attachments/assets/49b4f863-5fb0-4278-8308-608af3c1df04)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER

module halfadder(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule


HALF SUBRACTOR

module halfsubractor(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule

**RTL Schematic**


HALF ADDER

![WhatsApp Image 2024-12-04 at 16 10 58_ab025550](https://github.com/user-attachments/assets/6ec95753-c029-49ef-acd8-d95f10530252)


HALF SUBRACTOR

![WhatsApp Image 2024-12-04 at 16 12 16_a192e101](https://github.com/user-attachments/assets/9e54edf2-4f67-49c2-8def-7fda20853469)


**Output/TIMING Waveform**


HALF ADDER

![WhatsApp Image 2024-12-04 at 16 11 49_fb73cf73](https://github.com/user-attachments/assets/e73a330f-f99e-4d09-87d4-b8009b5defe8)



HALF SUBRACTOR

![WhatsApp Image 2024-12-04 at 16 13 31_ab72a1b9](https://github.com/user-attachments/assets/205f7f64-66ff-4c8f-a4b6-0fde48e0f2b6)


**Result:**

Thus the half adder and half subtractor circuit is designed and its truth table is verified in Quartus using Verilog programming .

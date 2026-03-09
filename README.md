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



**Truthtable**
Half Adder
<img width="424" height="249" alt="image" src="https://github.com/user-attachments/assets/6007fdb3-41e8-47e6-a875-3c03832c05e9" />

Half Subtractor
<img width="436" height="248" alt="image" src="https://github.com/user-attachments/assets/36d1687e-059e-4457-86ce-93c092b5a0f9" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:MUTHUAKASH M
RegisterNumber:212225230194
````
Half Adder:
````
module half(sum,carry,a,b);
output sum,carry;
input a,b;
assign sum=a^b;
assign carry=a&b;
endmodule
````
Half Subtractor:
````
module full(diff,borrow,a,b);
output diff,borrow;
input a,b;
assign diff = a ^ b;
assign borrow = ~a & b;
endmodule

````
**RTL Schematic**
Half Adder:
<img width="855" height="346" alt="image" src="https://github.com/user-attachments/assets/538b2dd8-8085-4f32-916b-b0950f338508" />
Half Subtractor:
<img width="827" height="368" alt="image" src="https://github.com/user-attachments/assets/2e45838c-821c-4461-beae-0460b8d54b19" />


**Output/TIMING Waveform**
Half Adder:
<img width="1919" height="475" alt="image" src="https://github.com/user-attachments/assets/9465c66a-ff8f-4221-bf09-3cac4272f2fa" />

Half Subtractor:
<img width="1919" height="341" alt="image" src="https://github.com/user-attachments/assets/7f05b73c-3d6d-44a0-ad4e-e72008b99775" />


**Result:**
Thus the Half Adder and Half Subtractor are studied and the truth tables are verified

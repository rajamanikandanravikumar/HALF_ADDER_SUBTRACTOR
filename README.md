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


**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)


**Truthtable**

![Screenshot 2025-05-06 083231](https://github.com/user-attachments/assets/ebd775a1-0649-4c66-9146-43fb81a12520)


![Screenshot 2025-05-06 083248](https://github.com/user-attachments/assets/5c2fa58e-addf-4d6d-bc40-4d728b74600f)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: Rajamanikandan R 
RegisterNumber:212223220082*/

Half Adder
```
module de3(a,b,sum,carry);
input a,b;
output sum,carry; 
 assign sum = a^b;
 assign carry = a & b;
endmodule
```
Full Adder
```
module de3(a,b,D,Bo);
input a,b;
output D,Bo; 
assign D = a ^ b;
  assign Bo = ~a & b;
endmodule
```

**RTL Schematic**
![image](https://github.com/user-attachments/assets/8aa6cc29-468d-4b46-8ca0-0971a6da38e2)


**Output/TIMING Waveform**
#### Half Adder
![image](https://github.com/user-attachments/assets/138a2eeb-77fc-4999-9332-12c9591c492b)

#### Full Adder
![image](https://github.com/user-attachments/assets/3f3d9421-d43d-438a-a090-3157c2167add)



**Result:**
The given logicate code is successfully verified using Verilog HTTP in QUTRUS II

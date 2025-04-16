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
![f241de15-1b34-4c76-ad5a-87c0beac0ace](https://github.com/user-attachments/assets/7c6bc521-46a5-40a5-b17b-6a0e06398e7d)

![16038998-403e-4ddd-8ca2-d7e62921f759](https://github.com/user-attachments/assets/484088f1-3688-45cb-b907-8a6c09db62ed)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
Developed by:Elamaran S E

RegisterNumber:212222230036*/
```
         module de(a,b,sum_a,carry_a,diff_s,borr_s);
         input a,b;
         output sum_a,carry_a,diff_s,borr_s;
         assign sum_a=a^b;
         assign carry_a= a&b;
         assign diff_s=a^b;
         assign borr_s=(~a&b);
         endmodule
```

**RTL Schematic**
![434127116-c1f0c226-8631-43d2-8af3-0921a92c746e](https://github.com/user-attachments/assets/0533d9c5-21ea-4bb6-8d15-84f14811af43)

**Output/TIMING Waveform**
![434127153-abe937bd-e340-4953-b0e4-fa7670132b3f](https://github.com/user-attachments/assets/05418f0c-b25d-42f2-99f4-fa3bbe5c624a)

**Result:**
Result: Thus, a half adder and half subtractor circuit has been implemented and it's truth table has been verified.



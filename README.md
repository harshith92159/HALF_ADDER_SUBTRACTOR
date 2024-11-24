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
![image](https://github.com/user-attachments/assets/7518510e-f2d8-4aee-9d8f-a030f2ce8262)
![image](https://github.com/user-attachments/assets/4dd03063-a24d-4b44-ac55-6637b8013127)
![image](https://github.com/user-attachments/assets/564808ae-366f-42bc-9e00-ab626b64338e)
![image](https://github.com/user-attachments/assets/aa19277f-686e-43a1-a75c-9b8833b11e57)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp5(din,a,b,c);
 input [0:7] din;
 output a,b,c;
 assign a=(din[4]| din [5]| din[6 ]| din[7]);
 assign b=(din[2]| din[3]| din[6]| din[7]);
 assign c=(din[1]| din[3]| din[5]| din[7]);
 endmodule
```

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:YUVA HARSHITH VARMA  RegisterNumber: 2300799

**RTL Schematic**
![Screenshot 2024-11-11 134736](https://github.com/user-attachments/assets/dabce1fd-4fd3-42bd-bb6d-afa1d6ed83c3)

**Output/TIMING Waveform**
![Screenshot 2024-11-11 134936](https://github.com/user-attachments/assets/4dd3c6fb-61c8-4546-bb38-36bac3783eb2)

**Result:**
Thus the Half Adder and HalfSubtractor circuits are designed and the truth tables is
 verified using Quartus software

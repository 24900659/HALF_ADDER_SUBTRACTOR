# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.
![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)
Sum = A’B+AB’ =A ⊕ B Carry = AB


Figure -01 HALF ADDER
![image](https://github.com/user-attachments/assets/f6abf561-2d06-4754-9fe5-94a8fd03258b)


**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 
![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)
Diff = A’B+AB’ =A ⊕ B
Borrow = A’B


Figure -02 HALF Subtractor
![image](https://github.com/user-attachments/assets/8e3f2a5c-3a0b-4743-ac3e-859fc9794c1c)

**Truthtable**
half adder
![image](https://github.com/user-attachments/assets/422a1bd0-291a-4207-a05f-c7dc7e8ba225)
half subtractor
![image](https://github.com/user-attachments/assets/3d217263-d96b-4051-b4fe-08c499ca497d)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
endmodule experiment3(a,b,cy,sm,df,bo);
input a,b;
output cy,sm,df,bo;
xor(sm,a,b);
and(cy,a,b);
xor(df,a,b);
and(bo,~a,b);
endmodule
```
```
Developed by:MOHANA K.V.S.L
RegisterNumber:24900659
```

**RTL Schematic**
![Screenshot 2024-11-05 111530](https://github.com/user-attachments/assets/b47dc618-9bc6-4cc3-a0e3-b3f7a1aa0a2b)

**Output/TIMING Waveform**
![Screenshot 2024-11-05 111814](https://github.com/user-attachments/assets/b91f027f-7127-4a4f-ae52-067eba5c7ffc)

**Result:**
HALF ADDER AND HALF SUBTRACTER IS DESIGNED AND THE TRUTH TABLE IS VERIFIED.

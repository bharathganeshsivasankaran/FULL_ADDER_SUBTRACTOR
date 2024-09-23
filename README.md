# EX04-FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

## AIM:

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

## Full Adder and Full Subtractor

## Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

## Figure -1 FULL ADDER

## Full Subtractor

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

## Truthtable

## Full adder

![image](https://github.com/user-attachments/assets/ac5b0de0-986f-4468-9edc-e34fc9a03ff3)

## Full subtractor
![318405667-33d8ba16-9169-40b0-8696-3bb8e5c3a0b7](https://github.com/user-attachments/assets/0dfbcd3d-fc55-4c1c-84aa-cb7b7bdbffeb)

## Procedure

```
1. Open Quartus Software   
2. Create a New Project  
3. Create a New Design File  
4. Compile the Program  
5. Generate RTL Schematic  
6. Create Nodes for Inputs/Outputs  
7. Generate Timing Diagram  
8. Simulate Different Input Combinations  
9. Save Your Work  
```

## Program:

```
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Bharathganesh S
RegisterNumber: 212222230022
```

```
module fulladdsub(a,b,c,sum,carry,diff,borrow);
input a,b,c;
output sum, carry,diff,borrow;
assign sum=(a^b^c);
assign carry=((a&b)|(a&c)|(b&c));
assign diff=(a^b^c);
assign borrow=((~a&b)|(~a&c)|(b&c));
endmodule

```

## RTL Schematic

![image](https://github.com/user-attachments/assets/1406b8e1-877a-40a5-a511-b22fc66da61e)


## Output Timing Waveform

![image](https://github.com/user-attachments/assets/5f218a52-0dd5-4789-bb2c-684861f4aa73)


## Result:

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.




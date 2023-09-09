# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Raja.R
RegisterNumber:  212222100041
# HALF ADDER
module Epo1(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum=A^B;
assign carry=A&B;
endmodule
# FULL ADDER
module Epoo1(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum=A^B^Cin;
assign carry =(A&B)|((A^B)&Cin);
endmodule
*/
Logic symbol & Truthtable
RTL realization
#HALF ADDER
![Screenshot 2023-09-02 092721](https://github.com/Raja8334/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120719634/9d926edb-22aa-4407-a5fd-d9443d4bf407)
#FULL ADDER
![Screenshot 2023-09-02 094051](https://github.com/Raja8334/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120719634/d2e59604-65f6-4c75-9aa2-88fdd619d3fe)


### Output:
### RTL
# HALF ADDER 

![Screenshot 2023-09-02 093727](https://github.com/Raja8334/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120719634/44b3d286-a4ac-4793-bdbc-8efc393d3e4e)
# FULL ADDER

![Screenshot 2023-09-02 094529](https://github.com/Raja8334/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120719634/16b7222f-4c98-4cd5-ba5d-73cc952929fd)


#


### TRUTH TABLE 
# HALF ADDER

![images (1)](https://github.com/Raja8334/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120719634/20172e9a-9c5b-419d-bc44-06093ae44748)

# FULL ADDER


![images](https://github.com/Raja8334/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120719634/a60ec817-a841-4abd-b8e8-1012edf874d3)



### Result:
Therefore,HALF ADDER and FULL ADDER are verified.

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
Developed by: M Chandru
RegisterNumber: 22008631
Half adder program:

module add(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

Full adder program:

module fulladd(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
*/
Logic symbol & Truthtable
RTL realization

### Output:
HALF ADDER
RTL realization:
![image](https://user-images.githubusercontent.com/119393023/213873314-1a70df4f-d09b-43de-aa9d-db9624064585.png)
FULL ADDER
RTL realization:
![image](https://user-images.githubusercontent.com/119393023/213873434-e0aba6a7-6a40-4d11-8b22-370c648001bb.png)

### TIMING DIAGRAM
HALF ADDER
![image](https://user-images.githubusercontent.com/119393023/213873671-b51dfa6c-190b-40c5-bbe4-f98c2afa876c.png)

FULL ADDER
![image](https://user-images.githubusercontent.com/119393023/213873275-8549329b-c4a2-4bac-8beb-f48d3e575f0d.png)
### TRUTH TABLE:
HALF ADDER
![image](https://user-images.githubusercontent.com/119393023/213873266-1e8203f9-a2e0-4789-9491-bda016abfd16.png)
FULL ADDER
![image](https://user-images.githubusercontent.com/119393023/213873462-0c8f8162-67e2-472a-96eb-8cf84c4ea5b9.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.

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
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Harini.M.D
RegisterNumber: 22001980

Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule

```

### Output:
HALF-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346502-9bef87a8-90a6-41d8-83c4-f68a4efa850a.png)
FULL-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346543-1478511e-7eb8-4795-a993-3c7b8dd6c52e.png)

### RTL
HALF-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346568-62ee200f-911f-4bcd-b250-599fab6b8641.png)
FULL-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346797-73acabba-5cc1-40ec-aed6-7950aa1ff3a1.png)

### TIMING DIAGRAM
HALF-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346838-a0ab7f4e-67a5-4050-8bbd-c3d732226725.png)
FULL-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346952-c6e35335-01b6-40da-b138-066ea4dcacdf.png)

### TRUTH TABLE 
HALF-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229346994-39f36ee3-0cf9-4320-af95-295a932ad950.png)
FULL-ADDER:-
![image](https://user-images.githubusercontent.com/113497680/229347032-2e49bafe-cc40-479f-a7f2-2eae6aa489d0.png)

### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.

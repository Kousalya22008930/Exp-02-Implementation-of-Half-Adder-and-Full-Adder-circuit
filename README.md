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

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
HALF ADDER:
module hh (a,b,s,c);
input a,b;
output s,c;
xor(s,a,b);
and(c,a,b);
endmodule

FULL ADDER:
module hh (a,b,bin,diff,bout);
input a,b,bin;
output diff,bout;
wire p,q,r,s,t;
xor(p,a,b);
not(q,a);
and(r,q,b);
xor(diff,p,bin);
not(s,p);
and(t,s,bin);
or(bout,t,r);
endmodule

Developed by: KOUSALYA A.
RegisterNumber:  212222230068
*/

### Output:
  HALF ADDER:
  ![Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit](half adder.jpg)
  ![Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit](half adder 1.jpg)

  FULL ADDER:
  ![Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit](full adder.jpg)
  ![Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit](full adder 1.jpg)




### Result:
Therefore using verilog programming in quartus for half adder and full adder circuit implemented successfully.
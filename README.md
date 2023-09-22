## Developed by: SANTHOSH S
## RegisterNumber: 212222100047
## Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
## Implementation-of-Half-Adder-and-Full-Adder-circuit

## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime Theory Adders are digital circuits that carry out addition of numbers.

## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/5636aad6-b580-4765-b907-a71f3dd94a06)

## Figure -01 HALF ADDER:
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/98483dd6-88ce-4806-8eef-e074308d766f)

## Figure -02 FULL ADDER
## Procedure
Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

## Program:
## Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
## Developed by: SANTHOSH S
## RegisterNumber: 212222100047
## HALF ADDER:
```
module exp33(a,b,s,c);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
```

## FULL ADDER:
```
module ass3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry= ((a&b)|(b&c)|(c&a));
endmodule
```
## Logic symbol & Truthtable RTL realization
## Output:
## RTL
## HALF ADDER:
![267980126-102cd944-2825-442a-a120-f7207350ca7d](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/fefdf702-329f-44b0-a93c-f7e82e32dafc)


## FULL ADDER:
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/b93e70e0-2105-4ac8-b450-1f41364db310)


## TIMING DIAGRAM:
## HALF ADDER:
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/b9d8baf4-dbfb-48d8-acaf-e88cf599aa1c)


## FULL ADDER:
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/18a9a39e-d678-4e9b-b1fe-eedd8646d1ca)


## TRUTH TABLE :
## HALF ADDER:
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/6085e167-6036-47c9-b46f-d35448699431)


## FULL ADDER:
![image](https://github.com/MrSanthosh-dev/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117916573/af330bd8-0d71-463f-851c-12d1bfa4f753)


## Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.

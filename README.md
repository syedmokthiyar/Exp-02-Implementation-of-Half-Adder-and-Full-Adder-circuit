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

### Procedure:
1. Connect the supply (+5V) to the circuit
2. Switch ON the main switch
3. If the output is 1, then the led glows.
### Program:
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.M.Syed Mokthiyar
RegisterNumber: 212222230156

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```
### TRUTH TABLE:
### Half Adder
![half adder exp3](https://github.com/syedmokthiyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118787294/a0a71b51-7db3-46d3-9f59-b765480c4d2d)

### Full Adder
![full adder exp3](https://github.com/syedmokthiyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118787294/db575bb6-a995-40b8-ae2e-af574d465613)

### RTL
### Half adder:
![RTL exp3 HA](https://github.com/syedmokthiyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118787294/fb6e2794-1093-477b-9a13-b5278962ba5c)
### Full adder:
![RTL exp3 FA](https://github.com/syedmokthiyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118787294/9d1eaf14-768c-45ba-b616-09612deab141)

## OUTPUT WAVEFORM:
### HALF ADDER
![OW Half exp3](https://github.com/syedmokthiyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118787294/d02ac90b-1f0d-4443-a2e6-7e9d1c5825c3)
### FULL ADDER
![OW full exp3](https://github.com/syedmokthiyar/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118787294/ea255276-fb86-4463-a828-5dc409841926)

### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.


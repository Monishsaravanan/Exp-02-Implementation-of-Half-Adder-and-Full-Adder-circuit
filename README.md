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
Developed by: THAMARAISELVAN V
RegisterNumber:  212221230115


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
## output
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: 
RegisterNumber:  
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL:
### Half Adder:
![image](https://github.com/Monishsaravanan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145743227/ca62916e-4293-4273-adbe-6deaf93737d9)

### Full Adder:
![image](https://github.com/Monishsaravanan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145743227/9a77e2a3-5165-47de-afba-f1fc3ff44fa3)

### TIMING DIAGRAM:

### Half adder:
![image](https://github.com/Monishsaravanan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145743227/011acd75-aebb-4f0d-9fbd-3e788fa96150)

#### Full adder:
![image](https://github.com/Monishsaravanan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145743227/90b29967-0602-4d2a-a8d8-bf0a870a274d)




### TRUTH TABLE :
### Half Adder:
![image](https://github.com/Monishsaravanan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145743227/8c977bb8-ec1a-40ed-b908-2e7f5ff7b602)

### full Adder:
![image](https://github.com/Monishsaravanan/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145743227/425fd7d9-876d-458b-b4c3-e513071c2891)



### Result:

## Name:R. sivakumar
## Reg:23013501

## Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

## Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

## Half Adder:
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder:
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

## Figure -01 HALF ADDER: 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

## Figure -02 FULL ADDER:

## Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
## Program:
## Half adder:

module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule

## Full adder:

module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule

## Logic symbol:

## Half adder:
<img width="324" alt="Screenshot 2023-12-18 123414" src="https://github.com/SIVAmech123/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629067/ab34987d-308d-4147-af2a-806f8f28674b">

## Full adder:

<img width="431" alt="Screenshot 2023-12-18 123433" src="https://github.com/SIVAmech123/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629067/13e6f115-148c-4dda-ae9b-1cdea04a9d94">

## Truthtable:

## Half adder:

<img width="363" alt="Screenshot 2023-12-18 123355" src="https://github.com/SIVAmech123/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629067/c2bc11fd-36b2-40b4-b5bd-8b1483b1ef48">

## Full adder:
<img width="495" alt="Screenshot 2023-12-18 123405" src="https://github.com/SIVAmech123/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629067/92e1c7f5-e0bb-4766-a7da-c2f291c96e4c">


## RTL realization:

## Half adder:
![WhatsApp Image 2023-12-18 at 13 16 42_37307859](https://github.com/SIVAmech123/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629067/0cfe1686-1bf7-4db7-993f-0dff0df68335)


## Full adder:
![WhatsApp Image 2023-12-18 at 13 17 50_521733d5](https://github.com/SIVAmech123/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151629067/a3597486-156d-4ba6-b671-edb04f6e5c08)

## Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

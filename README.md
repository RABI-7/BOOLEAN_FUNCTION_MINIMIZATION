### NAME : RABI BASKAR PRABURAJAN
### REGISTER NO : 24001812
### EXPERIMENT 2: BOOLEAN FUNCTION MINIMIZATION

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## EQUIPMENTS REQIURED :

Hardware – PCs, Cyclone II , USB flasher
SOFTWARE -QUARTUS PRIME:

## THEORY :

Implementing Boolean functions in Verilog HDL (Hardware Description Language) involves translating the simplified Boolean expressions into Verilog code to describe the behavior of digital circuits. The basic building blocks in Verilog is module. The module represent a combinational circuit. Use logical operators (&, |, ~, ^) to implement Boolean functions directly. Use built-in gate primitives for basic functions. Use University program VWF to verify the functionality of your Verilog modules. Create waveform and check outputs against expected results.



## PROCEDURE : 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## PROGRAM :

module EX2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;

output f1,f2;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

assign x1=(~a)&(~b)&(~c)&(~d);

assign x2=(~a)&(~c)&(~d);

assign x3=(~b)&(c)&(~d);

assign x4=(~a)&(b)&(c)&(~d);

assign x5=(b)&(~c)&(d);

assign x6=(x)&(~y)&(z);

assign x7=(~x)&(~y)&(z);

assign x8=(~w)&(x)&(y);

assign x9=(w)&(~x)&(y);

assign x10=(w)&(x)&(y);

assign f1=x1|x2|x3|x4|x5;

assign f2=x6|x7|x8|x9|x10;

endmodule



## TRUTHTABLE:
![WhatsApp Image 2024-12-02 at 13 51 28_014f8482](https://github.com/user-attachments/assets/8586e212-c322-47bf-9b92-b158222c9930)

## RTL OUTPUT :

![rtl 2](https://github.com/user-attachments/assets/8df23146-c1b3-4247-b2d7-3363e3f4a5c9)

## OUTPUT WAVEFORM:
![WhatsApp Image 2024-12-02 at 13 58 52_8bfb6a13](https://github.com/user-attachments/assets/17421960-f24e-442a-8b1b-b0e8bbf8d10b)


## RESULT :
       Thus the given logic functions are implemented using and their operations are verified using Verilog programming .


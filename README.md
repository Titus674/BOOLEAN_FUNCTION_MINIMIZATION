# BOOLEAN_FUNCTION_MINIMIZATION
## DEVELOPED BY: Titus ratna kumar karivella
## REGISTRATION NUMBER : 24002273

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:
```
module ex2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);

assign F1=x1|x2|x3|x4|x5;
endmodule
```
## RTL realization:
![image](https://github.com/user-attachments/assets/e44b812c-37af-4af1-aa14-de5bce29ad76)

## TRUTHTABLE:
![image](https://github.com/user-attachments/assets/60fb008a-bce7-4b10-ab80-acf66bb4e633)


## Timing Diagram:
![image](https://github.com/user-attachments/assets/db938942-1553-4c74-9c3f-7208fb5581cd)


## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


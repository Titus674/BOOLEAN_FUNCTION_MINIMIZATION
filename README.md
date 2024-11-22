# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: TITUS RATNA KUMAR KARIVELLA 
RegisterNumber: 24002273
```
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

```
**Logic & Truth Table**

![image](https://github.com/user-attachments/assets/e48aed94-4cfa-41cc-950b-b7a4f8ff3373)

![image](https://github.com/user-attachments/assets/e3cede7a-2ba5-4da2-a2db-9dd289a1c919)

**RTL realization**

![image](https://github.com/user-attachments/assets/2d95e4a5-1050-4e6e-af6f-87ac6d39567e)

**Output:**

![image](https://github.com/user-attachments/assets/8130f106-138b-4c16-9434-78ac9f0d2862)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


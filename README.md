
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Logic Diagram**

![image](https://github.com/user-attachments/assets/bc43e683-23af-4ecc-898f-8f65b50370be)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module exp2_1(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z,y;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: TITUS RATNA KUMAR KARIVELLA
RegisterNumber: 24002273*/


**RTL realization**

![image](https://github.com/user-attachments/assets/e570477d-1137-4210-8047-1c92c06839e4)


**Timing Diagram**

![image](https://github.com/user-attachments/assets/87b4f2a0-4c66-4075-80a0-9a8139e199f2)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


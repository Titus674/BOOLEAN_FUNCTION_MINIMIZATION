
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Logic Diagram**

![WhatsApp Image 2024-10-29 at 10 50 38_8dca61bb](https://github.com/user-attachments/assets/3bfa995f-5440-439c-9121-9139261fdb3d)


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

![Screenshot 2024-10-29 110615](https://github.com/user-attachments/assets/a00a52cd-4580-4950-8593-a25442041495)

**Timing Diagram**

![Screenshot 2024-10-22 111456](https://github.com/user-attachments/assets/8a3ca6fe-76b4-4eb3-8ff8-3aab7f6a8988)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


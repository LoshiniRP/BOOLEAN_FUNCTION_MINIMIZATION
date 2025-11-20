# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**EQUIPMENT REQUIRED:**

Hardware – PCs, Cyclone II , USB flasher

**SOFTWARE – Quartus prime**

**THEORY:**

**LOGIC DIAGRAM:**

**PROCEDURE:**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```

Developed by: RegisterNumber: 25002119

**RTL REALISATION OUTPUT:**
<img width="1920" height="1080" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/19185584-aa00-499c-a824-540972634bed" />

**RTL:**
<img width="1920" height="1080" alt="Screenshot (76)" src="https://github.com/user-attachments/assets/0cd9afde-cf69-4268-8425-516d32491b55" />

**TIMING DIAGRAM:**

**RESULT:**
Thus, the given logic functions are implemented using and their operations are verified using Verilog programming.

# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by   : GAYATHRI C
RegisterNumber : 25009125

module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule

*/

**Truth table**

![Truth table](https://github.com/user-attachments/assets/1baf2444-4493-4f11-b71f-27dcea85f83f)


**RTL realization Output:**
<img width="1024" height="883" alt="Screenshot 2025-11-21 093910" src="https://github.com/user-attachments/assets/64328e32-4be2-458d-bc4a-3560a67caa58" />


**Waveform Timing Diagram**
<img width="1919" height="629" alt="Screenshot 2025-11-21 152344" src="https://github.com/user-attachments/assets/2241d37a-0a39-44c8-ab44-04ba59cccc00" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


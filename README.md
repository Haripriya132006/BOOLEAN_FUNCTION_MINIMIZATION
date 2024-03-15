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
![Screenshot 2024-03-15 162844](https://github.com/Haripriya132006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870747/5a50362c-f0e9-4ce9-b697-771a1d988ccf)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
// Verilog model:Circuit with boolean expressions
module ex02 (E,F,A,B,C,D);
input A, B, C, D;
output E,F;
assign E = A || (B && C) || ((!B) && D);
assign F=((!B) && C) || ( B && (!C) && (!D));
endmodule
```
Developed by:HARIPRIYA K 
RegisterNumber:212223220030


**RTL realization**
![Screenshot 2024-03-15 155925](https://github.com/Haripriya132006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870747/74688d94-34c2-4668-ab5a-ea3a6bdeff90)



**RTL**
**Timing Diagram**
**Output:**
![Screenshot 2024-03-15 160303](https://github.com/Haripriya132006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870747/18eac204-35dd-4a05-83c1-d8fabe54f81d)






**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


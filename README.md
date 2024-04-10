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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. */
module ex02(a,b,c,d,w,x,y,z,f1,f2); 
input a,b,c,d,w,x,y,z;
output f1,f2; 
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u; 
not(adash,a); not(bdash,b); not(cdash,c);
 not(ddash,d);
 and(p,bdash,ddash);
 and(q,adash,b,d);
 and(r,a,b,cdash); 
 or(f1,p,q,r);
 not(ydash,y); 
 and(s,ydash,z); 
 and(t,x,y);
 and(u,w,y); 
 or(f2,s,t,u);
 endmodule
```
Developed by:HARIPRIYA K 
RegisterNumber:212223220030


**RTL realization**

![Screenshot 2024-04-10 113856](https://github.com/Haripriya132006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870747/6165149e-5930-46f3-97f2-4ef97728ce65)



**RTL**
**Timing Diagram**
**Output:**




![Screenshot 2024-04-10 114117](https://github.com/Haripriya132006/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870747/a1aacc77-a0d6-4887-8d75-f4e34f93b122)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


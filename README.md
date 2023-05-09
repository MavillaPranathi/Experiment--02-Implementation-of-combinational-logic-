# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce
one output.

Combinational logic gates are digital circuits that produce outputs based solely on the current inputs.
These gates are the building blocks for implementing digital systems and are used in a wide range of
applications, including arithmetic and logic operations, memory devices, and control circuits.

The two functions, F1 and F2, can be implemented using a combination of logic gates such as AND
gates, OR gates, and NOT gates.


## Procedure
1.Use module projname(input,output) to start the Verilog programmming.
2.Assign inputs and outputs using the word input and output respectively.
3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
4.Use each output(RTL Viewer and Timing Diagram) to represent F1 and F2.
5.End the verilog program using keyword endmodule.
## Program:
```
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by:m.pranathi
RegisterNumber:212222240064
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
module exp2f1(A,B,C,D,f1);
input A,B,C,D;
output f1;
assign f1=(~B&~D)|(A&B&~C)|(~A&B&D);
endmodule
F2=xy’z+x’y’z+w’xy+wx’y+wxy
module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=(~y&z)|(x&y)|(w&y);
endmodule 
*/
```
## RTL realization
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://user-images.githubusercontent.com/118343610/237052517-733b4352-694a-4dff-a9a0-987321fb35b2.png)


F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://user-images.githubusercontent.com/118343610/237052778-d17797dd-cc14-496e-8ce2-0ca3e58adf04.png)


## Output:
## TRUTH TABLE:
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://user-images.githubusercontent.com/118343610/237053232-b8cb5511-6806-4abb-898d-b44836805af5.png)


F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://user-images.githubusercontent.com/118343610/237053273-507a07c1-b201-4dfa-aa28-cc63f7a9374d.png)


## Timing Diagram
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://user-images.githubusercontent.com/118343610/237052864-f0c11ee3-341e-481f-a617-a1fb3a322f3d.png)


F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://user-images.githubusercontent.com/118343610/237052963-0978cb78-5194-49f7-992a-47581eda15a0.png)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.

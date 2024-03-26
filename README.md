# BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

## Software – Quartus prime

## Theory

## Logic Diagram

## Procedure

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

## Developed by: HARISHKUMAR R

## RegisterNumber: 212223230073

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

```py
module combinationalcircuit(A,B,C,D,F1);
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
## RTL realization

![image](https://github.com/harissunique/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139338/c0a8c18d-c433-4c69-8889-6a056abef8c1)



## Timetable
![image](https://github.com/harissunique/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139338/4e2cedcd-9a3f-43b4-820d-11ecc6422e8a)




## Timing Diagram

![image](https://github.com/harissunique/BOOLEAN_FUNCTION_MINIMIZATION/assets/147139338/4077835d-07bd-4b69-9307-a71df4b1aa0f)


## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


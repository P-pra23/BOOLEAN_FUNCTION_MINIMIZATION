# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Minimization F1**

![image](https://github.com/user-attachments/assets/2fdc20d7-d235-4804-af99-9fd21fcbd2e9)
![image](https://github.com/user-attachments/assets/50b2b55c-c6e6-4521-af52-868b53774afd)


**Truth table**

![image](https://github.com/user-attachments/assets/337527a4-fcac-40e2-b3f8-0206013652e3)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
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

Developed by:Prathikshaa.S  RegisterNumber:24007902


**RTL**

![image](https://github.com/user-attachments/assets/335f2f62-4692-4606-9fcb-38adbb4b2ef4)
![image](https://github.com/user-attachments/assets/7bd735af-078a-48b6-bcdc-4d3f4f989796)

**Output**

![image](https://github.com/user-attachments/assets/fe5af590-3cfc-41e9-96cb-438b7dece3b2)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


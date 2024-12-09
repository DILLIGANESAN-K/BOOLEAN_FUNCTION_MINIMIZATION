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
module exp_2(A, B,C,D,W,X,Y,Z,F1,F2); 
input A, B, C,D,W,X,Y,Z; 
wire w1,w2,w3,w4,w5,w6,w7,w8,w9,w10; 
output F1,F2; 
assign w1=(~A)&(~B)&(~C)&(~D);
assign w2=(A)&(~C)&(~D); 
assign w3=(~B)&(C)&(~D); 
assign w4=(~A)&(B)&(C)&(D);
assign w5=(B)&(~C)&(D); 
assign w6=(X)&(~Y)&(Z); 
assign w7=(~X)&(~Y)&(Z); 
assign w8=(~W)&(X)&(Y); 
assign w9=(W)&(~X)&(Y); 
assign w10=(W)&(X)&(Y); 
assign F1=w1|w2|w3|w4|w5; 
assign F2=w6|w7|w8|w9|w10; 
endmodule
```


Developed by:Dilli Ganesan RegisterNumber:24010195


**RTL realization**
![IMG-20241209-WA0030](https://github.com/user-attachments/assets/b00fe7d9-8900-410e-86d4-057f1df799e6)

**Output:**
![IMG-20241209-WA0031](https://github.com/user-attachments/assets/0494a802-7aa7-4519-a53a-2aaa5c7bf671)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


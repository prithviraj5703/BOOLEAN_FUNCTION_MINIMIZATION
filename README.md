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
```
1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.

```
**Program:**
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:V.PRITHVIRAJ 
RegisterNumber:212222100038
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

**RTL realization**
![312535957-dbd64921-6857-40ee-a21b-55fa17e9f89b](https://github.com/prithviraj5703/BOOLEAN_FUNCTION_MINIMIZATION/assets/121418418/a1e6c64e-b4ad-4203-b8cc-2cf7a7bc7ba4)

**TRUTH TABLE:**
![312536822-849f41b1-394f-48f4-b451-88315b927f79](https://github.com/prithviraj5703/BOOLEAN_FUNCTION_MINIMIZATION/assets/121418418/b6099408-9ab8-4d74-ac20-cd00030618d6)

**Timing Diagram**
![312537126-533d1307-308c-4a6d-9495-b6f289bf8479](https://github.com/prithviraj5703/BOOLEAN_FUNCTION_MINIMIZATION/assets/121418418/1ca4ba7d-c922-4e7f-a936-ef9d5ba37c36)

**Result:**
```
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


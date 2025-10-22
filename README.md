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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/212224230159

module booleanexpression ( input A, B, C, D, output F ); wire nB, nD, term1, term2, term3; // NOT gates not (nB, B); not (nD, D); // AND terms and (term1, nB, nD); // B'D' and (term2, A, C);
// AC and (term3, B, D);
// BD // OR the terms or (F, term1, term2, term3);


**RTL realization**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1ff53a2b-cbb5-450f-9388-63bf2e506c2a" />


**Output:**

**RTL**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d0143c31-0f94-4e67-bc23-6a236c353334" />


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
FULL ADDER
![WhatsApp Image 2025-12-05 at 09 34 56_51be57bd](https://github.com/user-attachments/assets/2a34a52c-c138-4527-9e3d-724e61672f84)

 FULL SUBRACTOR
 ![WhatsApp Image 2025-12-05 at 09 34 56_694f2328](https://github.com/user-attachments/assets/cf282508-dc9f-4673-9f79-75cded995511)

 



**Procedure**

Write the detailed procedure here
FULL ADDER:
1.Open Quartus II and create a new project.

2.Use schematic design entry to draw the full adder circuit.

3.The circuit consists of XOR, AND, and OR gates.

4.Compile the design, verify its functionality through simulation.

5.Implement the design on the target device and program it.

Full Subtractor:

1.Follow the same steps as for the full adder.

2.Draw the full subtractor circuit using schematic design.

3.The circuit includes XOR, AND, OR gates to perform subtraction.

4.Compile, simulate, implement, and program the design similarly to the full adder


**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by HARIHARAN M: RegisterNumber:25016362

FULL ADDER

module fa(a, b, cin, sum, carry);

input a, b, cin;

output sum, carry;

assign sum = (a ^ b) ^ cin;

assign carry = (a & b) | (cin & (a ^ b));

endmodule

FULL SUBRACTOR

module fs(a, b, bin, difference, borrow);

input a, b, bin;

output difference, borrow;

assign difference = (a ^ b) ^ bin;

assign borrow = (a & b) | (bin & ((a ^ b)));
*/

**RTL Schematic**
FULL ADDER
<img width="1902" height="768" alt="Screenshot 2025-12-05 081908" src="https://github.com/user-attachments/assets/92aacc88-a170-4db4-bb62-5863f55f6082" />
FULL SUBRACTOR
<img width="1905" height="765" alt="Screenshot 2025-12-05 081029" src="https://github.com/user-attachments/assets/cfa25f27-522b-4a27-a4bd-28d88cd62cdb" />



**Output Timing Waveform**
FULL ADDER
<img width="1906" height="373" alt="Screenshot 2025-12-05 082212" src="https://github.com/user-attachments/assets/25b2ee13-d6db-4f58-a6f2-f725169a5ed5" />
FULL SUBRACTOR
<img width="1910" height="426" alt="Screenshot 2025-12-05 081259" src="https://github.com/user-attachments/assets/ec6df59a-0770-429e-851d-b13fee8c6893" />



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.




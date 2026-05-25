# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**
```
module ex3(sum, carry, a, b, cin);
    output sum;
    output carry;
    input a;
    input b;
    input cin;

    assign sum = a ^ b ^ cin;
    assign carry = (a & b) | (cin & (a ^ b));
endmodule
```

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**
```
module ex3sub(diff, borrow, a, b, bin);
    output diff;
    output borrow;
    input a;
    input b;
    input bin;

    assign diff = a ^ b ^ bin;
    assign borrow = (a & b) | ((a ^ b) & bin);
endmodule
```

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

## full adder##

<img width="1920" height="1080" alt="Screenshot (95)" src="https://github.com/user-attachments/assets/d74b1ecc-dee4-4474-bb98-1f02a6528e4b" />
## full subractor##
<img width="1920" height="1080" alt="Screenshot (97)" src="https://github.com/user-attachments/assets/5d577562-57d5-45df-bd02-2ace3eddfb21" />
## full adder##
<img width="1920" height="1080" alt="Screenshot (96)" src="https://github.com/user-attachments/assets/af381b9e-36c8-4550-9802-282a9f242923" />
## full subractor##
<img width="1920" height="1080" alt="Screenshot (98)" src="https://github.com/user-attachments/assets/3a6e65c0-abef-4fa3-b75a-392524697b06" />



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.




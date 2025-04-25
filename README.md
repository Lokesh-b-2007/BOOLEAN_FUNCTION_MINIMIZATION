
BOOLEAN_FUNCTION_MINIMIZATION
AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

F2=xy’z+x’y’z+w’xy+wx’y+wxy

Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

Theory  ![426922546-e95b143e-8dca-4431-9f51-7585f5e1c0b0](https://github.com/user-attachments/assets/35958aa7-10b9-47d8-b4f7-c348f0439ba4)


Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: Lokesh B reg.no:-212224040172
~~~
module ex2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule
module ex2_2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&z)|(x&y)|(w&y&~z));
endmodule
~~~
RTL realization

1-a)
![426923015-649cc145-ba52-4298-9cb6-2fca77af9897](https://github.com/user-attachments/assets/f57bf1f0-0d14-4dda-9a0d-0eb3d059fbe6)


1-b)
![426923460-3854152f-2b1d-4a1b-8497-9a9fe5771b17](https://github.com/user-attachments/assets/29b4549c-d87f-4911-aa0d-d0523ffb213a)


Timing Diagram

2-a)
![426923986-0b3f910e-0f1f-43c2-a9dc-9c663001e820](https://github.com/user-attachments/assets/65601282-72f1-453e-87d9-b844f97aa501)


2-b)
![426926401-7aa0b28d-f3cb-4b51-b518-c08af29634a1](https://github.com/user-attachments/assets/047de71d-893f-4a62-99d3-74ce0837b064)


Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

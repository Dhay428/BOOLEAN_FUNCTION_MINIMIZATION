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

FUNCTION 1 K-MAP
![Screenshot 2024-12-08 213046](https://github.com/user-attachments/assets/8fb6d444-32ea-4c7f-9c97-dc037ce00090)

FUNCTION 2 K-MAP

![Screenshot 2024-12-08 213054](https://github.com/user-attachments/assets/9f556e5e-0fc5-48c7-a959-f5c20f7a5786)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
FUNCTION 1

![Screenshot 2024-12-08 213106](https://github.com/user-attachments/assets/f5beac3b-fde2-445c-a480-7348fae63790)


FUNCTION 2

![Screenshot 2024-12-08 213113](https://github.com/user-attachments/assets/061076fd-f820-4102-9bd9-a64083e840fa)

Developed by : Dhayalaprabu.S

RegisterNumber:24006289


**RTL realization**

**Output:**

**RTL**

FUNCTION 1
![Screenshot 2024-12-08 213120](https://github.com/user-attachments/assets/f912b38a-ef8d-4af3-bca8-306ff7b2e9f8)

FUNCTION 2

![Screenshot 2024-12-08 213129](https://github.com/user-attachments/assets/62e3b8b7-c489-4ef7-a4ae-bc7897e350d9)

**Timing Diagram**
 FUNCTION 1
 ![Screenshot 2024-12-08 213652](https://github.com/user-attachments/assets/0204f563-4947-4272-8b8b-4480f0b01d3c)

 FUNCTION 2
 ![Screenshot 2024-12-08 213700](https://github.com/user-attachments/assets/470a1150-b3a6-4433-87a8-fa3533d6d917)



 
**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


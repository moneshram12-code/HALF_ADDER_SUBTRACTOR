# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

Half Adder Truthtable : 

  ![tt](https://github.com/user-attachments/assets/3218cab7-3402-4f43-b268-36472166f1c6)
 

    
Half Subtractor Truthtable :

   ![half subtractor tt](https://github.com/user-attachments/assets/7c2fe8ff-1630-4e7f-add1-96ca5b67a695)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming

1)
 Half Adder
  
    module half_adder (
       
       input wire a, b,   //Inputs
       
       output wire sum,    //sum output
       
       output wire carry,  //carry output
     );

       //Logic equation

       assign sum = a ^ b;  //XOR for sum
       
       assign carry = a & b; //AND For carry

      endmodule

1)

  Half Subtractor

    module half_subtractor (
     
     input wire a, b,          //Inputs
     
     output wire diff, borrow  //Outputs
    );
     
      // Logic equations 
      
      assign diff   = a ^ b;        //  XOR for difference
      
      assign borrow = ~a & b;       // Borrow when a < b
      
   endmodule  

Developed by: Monish . R

RegisterNumber: 250147815

**Output/TIMING Waveform**

Half Adder :

 ![half adder ](https://github.com/user-attachments/assets/b384baef-ee64-4410-b3a0-f09d2d7dc76b)

Half Subtractor :

  ![half subtractor](https://github.com/user-attachments/assets/b7bc741d-b03c-4585-9629-36fae0c7b4b8)

Timing WaveForm:

   ![op1](https://github.com/user-attachments/assets/1d267a5c-a924-472f-9731-8e08a9288a66)

Timing Waveform:

   ![op2](https://github.com/user-attachments/assets/ffdaf1cc-bbf7-478d-9f8b-651d76cb0d72)




**Result:**

   Designing a half adder and half subtractor circuit and verifying its truth table in Quartus using Verilog programming is created successfully

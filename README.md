# Implementaion-of-AND-gate-using-NOR-gate
# AIM:
To design a AND gate using NOR gate and verify its truth table in Quartus using Verilog programming.

# HARDWARE REQUIRED:
PC
Cyclone II
USB flasher

# SOFTWARE REQUIRED:
Quartus prime Model Sim

# Theory
## AND GATE: 
AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB

Boolean Expression Y = A.B

![AND gate diagram](https://user-images.githubusercontent.com/118707693/213923370-e508f517-7dde-40b0-8ca0-81d7ddc0df8c.png)



## NOR GATE:
This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.

Boolean Expression Y = (A+B)'

![nor gate](https://user-images.githubusercontent.com/118707693/213923350-7fdfe8b7-c0f1-4925-bb22-de0f010fd274.png)


# Explanation:
An AND gate is equivalent to an inverted-input NOR gate. A NOR gate is equivalent to an inverted-input AND gate. An OR gate is equivalent to an inverted-input NAND gate. Two NOT gates in series are same as a buffer because they cancel each other as A'' = A.

### AND gate using NOR gate:-
#### proof:-

(A+A)' = A' similarly, (B+B)' = B'
so, (A'+B')' = (A.B)'' (Demorgain Law)
= A.B

![and-nor diagram ](https://user-images.githubusercontent.com/118707693/213922690-bde57394-49ae-47e8-8c3f-b7a489d5da83.png)


# Procedure:

1.start the module using module projname().

2.Declare the inputs and outputs.

3.Use wire to assign intermediate outputs.

4.Use NOR gates to get the desired output.

5.End the module.

6.Generate RTL realization and timing diagrams.

# Program:
```
Program to verify the truth table in quartus for the basic logic gates using Verilog programming.
Developed by: A.Thiyagarajan
RegisterNumber: 22008681

module andnor(A,B,Y);
input A,B;
output Y;
wire P,Q;
nor(P,A,A);
nor(Q,B,B);
nor(Y,P,Q);
endmodule
```
# Output:

## RTL diagram
![and-nor rtl](https://user-images.githubusercontent.com/118707693/213922813-86c3ad2b-c4c8-42d9-b689-5841de1e98c8.jpg)


## RTL Timing diagram
![and-nor td](https://user-images.githubusercontent.com/118707693/213922825-245eb0ca-2703-47a6-a13a-086fc2aa366d.jpg)



# Result:
Hence AND gate using NOR gate has been implemented and verified using verilog programming and its output are validated.








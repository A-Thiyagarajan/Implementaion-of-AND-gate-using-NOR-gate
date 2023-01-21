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

## NOR GATE:
This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.

Boolean Expression Y = (A+B)'

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


# Result:
Hence AND gate using NOR gate has been implemented and verified using verilog programming and its output are validated.








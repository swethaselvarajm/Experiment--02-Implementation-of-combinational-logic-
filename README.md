# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime

## Theory
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

###Using NAND gates: NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'

## Logic Diagram
Using NOR gates NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'

## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: SWETHA.S
RegisterNumber: 212222230155

![Screenshot 2023-08-28 225513](https://github.com/swethaselvarajm/Experiment--02-Implementation-of-combinational-logic-/assets/119525603/779a0795-41f4-4134-87ef-8665b71d7be0)
*/

## Output:
## RTL

![Screenshot 2023-08-26 095603](https://github.com/swethaselvarajm/Experiment--02-Implementation-of-combinational-logic-/assets/119525603/7b295287-fe76-408c-82a1-7ccaacf8c8c8)

## Timing Diagram

![Screenshot 2023-08-26 095627](https://github.com/swethaselvarajm/Experiment--02-Implementation-of-combinational-logic-/assets/119525603/4e17c3af-bfd9-4c3b-a91c-20d8b956c79b)

## Truth Table

![Screenshot 2023-08-26 095708](https://github.com/swethaselvarajm/Experiment--02-Implementation-of-combinational-logic-/assets/119525603/0e36923d-af5f-4da7-af56-fdcbb176b542)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.

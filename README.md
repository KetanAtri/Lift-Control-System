# Lift-Control-System
A lift control system has been designed using multiplexers (I worked on the implementation as well). The circuit designed here is 
capable of deciding which lift should respond when the user presses the call button on any floor. The software "Logisim" was used
for the simulation of the circuit and files for the same have been given in the repository.

## Features
1. Designed for a building with 4 floors, logic is extensible for more floors
2. Lift overload (due to excess weight) is taken under consideration while deciding the respondant lift
3. Preferential response of lifts saves energy by using the force of gravity when possible
4. Implementation can be done using multiplexers alone

## Assumptions
1. Only one user presses the call button at a given time
2. Overloaded lift (due to weight) will not respond to call on any floor

## Limitations
1. Lift response follows First Come First Serve model
2. Circuitory designed and implemented only for decision making (separate from lift control circuitry)
3. For more floors the circuitry grows more complex

## File Descriptions
### Truth Table.xlsx
This file creates the truth table for the logic of the circuit which will be used. In the file following variables have been used:
AB - Floor indicator for Lift 1 (0 to 3)
CD - Floor indicator for Lift 2
EF - Floor indicator for Call Button
Wa - Weight overload indicator for Lift A (1 for overload)
Wb - Weight overload indicator for Lift B

### Lift Control[FINAL].circ
This file (XML type) containes the implemented circuitry. If used with the "Logisim" software it provides interactivity tool as well
which allows for observing the working of the circuit.

# hardware_assignment
# H-Bridge Circuit for DC Motor Directional Control

## 1. Project Overview

This project involves the design and simulation of an H-bridge circuit in Proteus for controlling the direction of rotation of a DC motor. The circuit allows the motor to rotate in both forward and reverse directions by changing the polarity of the voltage applied across its terminals.

The H-bridge consists of four transistors arranged around the DC motor. By switching specific pairs of transistors ON and OFF, the direction of current through the motor can be controlled without physically changing its connections.

## 2. Components Used

The following components were used in the circuit:

- Four transistors: i used a BC547 NPN resistor for the bottom part,BC557 PNP resistor for the upper pair Used as electronic switches to control the current flowing through the motor.
- **Four 1 kΩ resistors:** Used as base resistors to limit the current entering the transistor bases, subject to the requirements of the final circuit.
- **One DC motor:** The output device whose direction of rotation is controlled.
- **DC power supply:** Provides the electrical energy required to operate the circuit.
- **Ground terminal:** Provides the common reference point for the circuit.
- **Proteus Design Suite:** Used to draw the circuit schematic and simulate its operation.

### Note on Transistor Selection

During the initial design, four 2N5772 transistors were used. The transistor selection was later changed to BC557 PNP transistors for the upper pair and BC547 NPN transistors for the lower pair.

This change was made to implement a conventional complementary-transistor H-bridge arrangement. The selected transistors must have suitable current and voltage ratings for the motor, and the base resistors must be appropriate for the required operating current.

## 3. How the Circuit Works

The H-bridge operates by controlling four transistors positioned around the DC motor. The upper transistors connect the motor terminals towards the positive supply, while the lower transistors connect them towards ground.

When an appropriate diagonal pair of transistors is switched ON, current flows through the motor in one direction. When the opposite diagonal pair is activated, the current flows through the motor in the opposite direction.

Since the direction of current determines the direction of rotation of a conventional DC motor, reversing the current reverses the motor's rotation.

The transistors function as electronic switches, while the resistors help control the base current required to operate them.

## 4. How Directional Control Was Achieved

Directional control was achieved by switching different diagonal pairs of transistors.

**Forward Rotation:** One diagonal pair of transistors is switched ON while the other pair remains OFF. This causes current to flow through the motor in the forward direction.

**Reverse Rotation:** The first pair is switched OFF, and the opposite diagonal pair is switched ON. This reverses the current through the motor, causing it to rotate in the reverse direction.

**Stopping the Motor:** All four transistors are switched OFF, allowing the motor to coast to a stop.

Care must be taken to ensure that both transistors in the same bridge leg are never switched ON simultaneously, as this can create a short circuit between the positive supply and ground.

## 5. Simulation Procedure

The circuit was designed in Proteus by placing the transistors, resistors, DC motor, power supply and ground terminals on the schematic workspace. The components were then interconnected to form the H-bridge configuration.

The circuit's directional control was evaluated by changing the transistor control states. The expected forward and reverse operating conditions were examined by activating the appropriate diagonal pairs.

Screenshots of the completed schematic and the two directional operating states can be included as evidence of the simulation results.

## 6. Conclusion

The project demonstrates the operating principle of an H-bridge circuit and its application in controlling the direction of rotation of a DC motor. By switching the appropriate diagonal transistor pairs, the polarity of the voltage applied to the motor can be reversed, enabling forward and reverse rotation.

The project also provides practical experience in transistor switching, circuit design, component selection and electronic circuit simulation using Proteus.

With love, Zainab 😊

# Two-stage-opamp-design-in-cadence
A simulation project that was implemented and analyzed using the Cadence tool.   The Gpdk90 library has been used for the designing of the circuit.
# The project is based on a IEEE paper on Electronics, Information & Communication Technology
The project proceeds in the following manner

1) ABSTRACT
2) BASIC CIRCUITS USED
3) PROBLEM STATEMENT
4) PROPOSED TECHNIQUE
5) ScHEMATIC DIAGRAM
6) SIMULATION RESULT
7) CONCLUSIONS

# Abstract
A differential amplifier is actually a electronic amplifier which amplifies the difference 
between two input voltages and suppresses any voltage common to the two inputs. 
Differential type amplifier is a analog circuit in which there is two input terminal and 
one output terminal. The input is actually the difference between the value of two
input terminals. The differential amplifier is a vast used circuit building block in analog
integrated circuits, principally op-amps. 
The differential amplifier can be implemented with BJTs or MOSFETs. Here we have 
got high gain of 61 dB .
It was seen that two stage amplifier gives better amplification because of the 
multiplying factor. Here we have taken some specification based on which we derived
the results theoretically and then simulated in the order to get the results. Here in our
proposed circuit we have got very good CMRR of 75dB.

# PROBLEM STATEMENT
• The gain and CMRR obtained by using a single stage differential amplifier does not match the 
requirements of the practical applications.
• Hence we go for a two stage differential amplifier where the first stage will be a differential pair 
Which is used to reduce the noise in the signal to be amplified and the second stage will be used for the 
purpose of increasing the gain of the amplifier
• The problem with the actual two stage operational amplifier is that is has least phase margin 
which is not suitable for practical applications
An operational amplifier is said to be good if it has following specifications
\n• High Gain and CMRR
\n• High input impedance
\n• Good phase margin (400 − 600)

# BASIC CIRCUITS USED




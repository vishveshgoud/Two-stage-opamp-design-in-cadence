# Two-stage-opamp-design-in-cadence
A simulation project that was implemented and analyzed using the Cadence tool.   The Gpdk90 library has been used for the designing of the circuit.
# The project is based on a IEEE paper on Electronics, Information & Communication Technology
The project proceeds in the following manner

1) ABSTRACT
2) BASIC CIRCUITS USED
3) PROBLEM STATEMENT
4) PROPOSED TECHNIQUE
5) SCHEMATIC DIAGRAM
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
The gain and CMRR obtained by using a single stage differential amplifier does not match the requirements of the practical applications.
Hence we go for a two stage differential amplifier where the first stage will be a differential pair Which is used to reduce the noise in the signal to be amplified and the second stage will be used for the purpose of increasing the gain of the amplifier.
The problem with the actual two stage operational amplifier is that is has least phase margin which is not suitable for practical applications.

An operational amplifier is said to be good if it has following specifications
 1) High Gain and CMRR
 2) High input impedance
 3) Good phase margin (400 − 600)
# BASIC CIRCUITS USED
1) Current mirror circuit

    ![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/57cd7709-c6e2-4064-b5d3-ff71f5665d75)

   The main purpose of using these current mirror circuit is to copy the current in one barnch to another branch by taking proper W/L ratios of the two mosfets M1 and M2
   we can replicate the currents.

2) MOSFET COMMON SOURCE AMPLIFIER:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/e553415f-879e-4255-b4ff-8067463eb6c8)

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/bc883219-d351-409d-9695-16a14e9ab88e)


3) BALANCED OUTPUT DUAL INPUT DIFFERENTIAL AMPLIFIER(BJT):

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/ada08843-be06-4af9-9efe-fa072b8299a2)


![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/32903fc9-a6cb-45b3-80f8-361b60595253)

4) SMALL SIGNAL ANALYSIS OF SINGLE STAGE :                                                  

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/ccd03b7a-2a57-4b03-aa19-d6619536d0c8)

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/53d38ba5-8f41-4659-9e41-d3912eefbab5)

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/6673f68f-9eaa-41ec-bf4a-b5f5eb5ff27a)

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/e4cb2c15-0a84-4e5d-965f-089883f4d2c2)

5) TWO STAGEE OPERATIONAL AMPLIFIER :

   ![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/75d312e2-825c-4818-ae41-b219e146d7c2)

   ![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/c63890a9-b5bf-416a-96ca-0144790c519a)

   ![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/db447797-5801-4f53-bf0e-8c67b13abee0)

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/d2839947-b01e-45e3-8ab7-188ba3ce08ba)

# PROPOSED TECHNIQUE

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/bf2a6ad7-69fc-4683-9208-3094e8225021)

MILLER EFFECT:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/2b4aad1e-6e4c-4500-94c8-719968a6dac0)

By using small ‘C’ we can get larger value of ‘C’ by 
miller effect. 
 It is used for better phase margin. If p1(pole 1)
 can be shifted towards left and p2(pole 2) can be shifted 
towards right then phase margin will be better. As we 
can see in the diagram above the effect of capacitance 
“C” in pole P1 & P2, by implementing in P1 the pole 
shifts greatly towards left and P2 shifts towards right. 
So here miller capacitor is being used to get good 
phase margin.

The proposed circuit diagram:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/0e32bb31-9804-46cf-bc3a-4a88d463e8bb)

# SCHEMATIC DIAGRAM
The design is implemented using 90 nm technology in Cadence using gpdk90 library the width and lengths are taken as per the specifications given in the paper.
Below table shows the lengths and width Of the various mosfets used in the circuit:

<img width="494" alt="table" src="https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/0fb2c02f-f9f7-44f1-95f1-dac1626b0df9">

Single stage Schematic diagram:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/bd7b4a86-e4d2-468b-8408-dc76e9d5c9cc)

Two stage Schematic diagram:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/d56d8594-82b2-42dd-9ff1-75ecc7a9a7bf)

# SIMULATION RESULT
Input and Output waveforms of single stage opamp:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/020a82f5-955d-441d-b37f-278890f613cf)

Input and Output waveforms of final two stage opamp:

![image](https://github.com/vishveshgoud/Two-stage-opamp-design-in-cadence/assets/147975068/4f868019-6f33-4ca2-a3f2-e625f6cf9bde)

Gain and CMRR Calculations:

Differential mode:		

V1 = 1 mV pk-pk 1kHz     

V2= 0.4 mV pk-pk 1kHz

Vin = V1-V2= 0.6 mV pk-pk

Vout = 664 mV pk-pk (from the graph)

Gain = 𝑉𝑜𝑢𝑡/𝑉𝑖𝑛=664/0.6=1106

Gain in dB = 20log_10⁡1106 = 60.88 dB

common mode:

V1 = 1 mV pk-pk 1kHz

V2 = 1mV pk-pk  1kHz

Vin = (𝑉1+𝑉2)/2  = 1 mV pk-pk

Vout = 0.2 mV pk-pk (from the graph)

Gain = 𝑉𝑜𝑢𝑡/𝑉𝑖𝑛=0.2/1=0.2

Gain in dB = 20log_10⁡0.2 =-14  dB

CMRR=𝐴_𝑑/𝐴_𝑐  =  1106/0.2 = 5530

CMRR in dB = 74.8dB

# CONCLUSION

The two stage operational amplifier was simulated in cadence with gpdk90nm technology.
After simulating the proposed circuit we have got high gain of 
61dB with several other good parameters. CMRR of   75dB  . the response of the circuit is very high as a result its gets an edge over other circuits and the CMRR with the proposed technique increases its value. 




































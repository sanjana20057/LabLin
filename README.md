# LabLin
exploring and implementing integrated circuits!!


CS Amplifier:

> a common-source amplifier is one of three fundamental single-stage field-effect transistor (FET) amplifier configurations, most commonly employed as a voltage or transconductance amplifier. 

>In this case, the signal comes in on the gate, and goes out on the drain. The terminal in left is the source. This is a common-source FET circuit. The corresponding BJT circuit can be considered to be a transconductance amplifier or a voltage amplifier.

>Here input voltage controls the current through the FET, varying the voltage across the output resistance. But the output resistance of the FET device is usually not high enough to be a good transconductance amplifier, nor low enough to be a good voltage amplifier(zero).

operations:








key features:

>Gain:

The gain of a MOSFET is dependent on the transconductance and drain resistor value. The highest gain of an individual MOSFET is referred to as the intrinsic gain.

  Transconductance: The transconductance depends on the bias point.

  Drain resistor: The drain resistor value is directly proportional to the voltage gain of a MOSFET amplifier.

  Intrinsic gain: The intrinsic gain is the highest gain of an individual MOSFET transistor. It is determined by the 
  product of the transconductance and the output impedance of the MOSFET.

  Gain at low frequency: The gain at low frequency is influenced by coupling capacitors.

  Gain at high frequency: The gain at high frequency is lowered by parasitic capacitance.


>Phase shift:

 output is 180 degree out of phase with input signal.


>Frequensy response:

   1. For high frequencies gain decreases due to capacitors.
     
   2. For low frequencies gain drops due to miller effect.
     
   3. In mid band frequency gain is stable.


>Power consumption:

 consumes less power making it suitable for operations done using battery.


>Impedence:

 Input impedence: a high input impedence prevents signal loss due to loading.
 
 Ouput impedence: low output impedence ensures efficient signal transfer with minimal loss.     


 >Applications:

1. Audio Amplification
   
 • Utilized in microphone preamplifiers and low-power audio circuits.
 
 • It boosts weak audio signals prior to driving a power amplifier or speaker.
 
 • Supplies high voltage gain to increase low-amplitude signals.

2. RF (Radio Frequency) and IF (Intermediate Frequency) Amplifiers
   
• Utilized in radio receivers, transmitters, and communication equipment.

• Amplifies weak RF signals for more effective signal processing and transmission.

• Provides good voltage gain with high input impedance, essential for RF applications.

3. Sensor Signal Conditioning
   
• Employed in photodiodes, biosensors, and temperature sensors for amplifying low-level signals for subsequent processing.

• Present in medical devices (ECG, EEG) and industrial sensors.

• High input impedance minimizes sensor loading.

• Amplifies sensor voltages which are very low for measurement in an accurate sense.

4. Analog Signal Processing
   
• Implemented in mixers, modulators, and demodulators used in communication equipment.

• A component of oscillators and filters in electronic systems.

• Gain as well as its frequency response suits it for effectively processing analog signals.

5. Buffer and Driver Circuits
    
• Utilized as an intermediate stage between high-impedance sources and low-impedance loads.

• Assists in driving next-stage circuits such as power amplifiers or ADCs (Analog-to-Digital Converters).

• Delivers required voltage amplification while preserving signal integrity.

6. Video Amplifiers
    
• Utilized in TV receivers, cameras, and display systems to amplify video signals.

• Assists in enhancing video quality and transmission range.

• Can handle high-frequency signals with acceptable gain.

7. Wireless and Bluetooth Communication

• Used in RF front-end circuits to amplify signals in Bluetooth, Wi-Fi, and cellular communication.

• Suits high-frequency applications with appropriate impedance matching.


 EXPERIMENT:

 Aim: to determine drain current of nMOSFET and observe the variation in drain current when we vary the parameters of 
 MOSFET. To do ac analysis, dc analysis and transient analysis.


 ![image](https://github.com/user-attachments/assets/0d2cb143-3bd1-4c14-8f5b-b1832e03a15a)

 DC Analysis:


 ![50u1](https://github.com/user-attachments/assets/7c6236de-3033-4662-93a8-1b70c9445484)

 Case1: when width is 1um
 
 ![image](https://github.com/user-attachments/assets/1bb1700f-2620-4496-b4f1-09166ae987a0)

 Case 2: when width is 2um

![image](https://github.com/user-attachments/assets/4aaf273d-1243-49f1-81f6-0390d42f7f90)


 Inference: in case 1 and 2 we can observe that i hve doubled the width of the channel so crrespondingly the is increase in the case 2 because as width of the channel increases the number of charges flowing through the channel also increases so due to increase in widths so current also increases.
 

 AC Analysis:
 
1.
 ![ac1](https://github.com/user-attachments/assets/bb3d24dd-9a0c-44a9-9a90-9218c14f67cd)
 
2.
 ![ac2](https://github.com/user-attachments/assets/60360546-f4c2-46c3-908d-f3ee1b2903bb)

1. Gate Voltage (First Image):
   
	•	The gate waveform has a greater amplitude, which means that the input signal is properly connected to the MOSFET.

	•	This implies little or no attenuation at the gate terminal, as would be expected, because it is driven directly by the input source.

2. Drain Voltage (Second Image):
•	The drain waveform has a much smaller amplitude than the gate voltage.

• This can mean that the MOSFET is only giving reduced gain, probably because of the short  channel length (180 nm), which may cause short-channel effects that compromise its amplifying ability.

• The attenuated amplitude also indicates a high output impedance or reduce transconductance, which compromises the signal strength at the drain.

Conclusion:

•The MOSFET acts as an amplifier, but the short channel width (180 nm) can be restricting its gain, and it is therefore not producing as large a drain voltage amplitude.

•The fact that the drain signal is less than the gate signal suggests that the circuit can be optimized, i.e., make the transistor wider or alter the biasing conditions to maximize the gain. 


 Transient analysis:

![image](https://github.com/user-attachments/assets/e62a12af-ba65-46e1-8432-3bae9612b4e9)


![image](https://github.com/user-attachments/assets/e326c897-43c3-4b47-8fa8-9043bcf27101)

![image](https://github.com/user-attachments/assets/15165f01-fb7a-49a1-b45c-7be8b6d80f2b)


1. The output voltage not only gets inverted but also experiences a boost in amplification. This happens because when you crank up the gate voltage, the drain current rises, leading to a voltage drop across the drain resistor.

2. The waveform comes out smooth, which means there's hardly any distortion and the amplification remains linear. This is thanks to the absence of channel length modulation.

3. You'll notice a 180-degree phase shift between the input and output signals. This phase flip occurs because increasing the gate voltage results in a drop in drain voltage, effectively inverting the output.




QUESTION 2:

DC Analysis:

 ![dc](https://github.com/user-attachments/assets/06c60166-1f49-4920-8ea9-f70b8afdaf7e)

AC Analysis:

 ![ac](https://github.com/user-attachments/assets/92ceed7e-0031-49ae-b8c5-2bf401a972fe)

Transient Analysis:

 ![tansient](https://github.com/user-attachments/assets/9ff063f2-b200-4021-868c-2ff6a5b86079)





 




 
 

     
     
     



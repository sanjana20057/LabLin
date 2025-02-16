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


Phase shift: output is 180 degree out of phase with input signal.


Frequensy response: 
   1. For high frequencies gain decreases due to capacitors.
     
   2. For low frequencies gain drops due to miller effect.
     
   3. In mid band frequency gain is stable.


 Applications:









 EXPERIMENT:

 Aim: to determine drain current of nMOSFET and observe the variation in drain current when we vary the parameters of 
 MOSFET. To do ac analysis, dc analysis and transient analysis.


 ![image](https://github.com/user-attachments/assets/0d2cb143-3bd1-4c14-8f5b-b1832e03a15a)

 DC Analysis:


 ![50u1](https://github.com/user-attachments/assets/7c6236de-3033-4662-93a8-1b70c9445484)

 Case1: when width is 50um
 
 ![50u](https://github.com/user-attachments/assets/e30541e4-076b-4acd-8492-49c037cd1cd5)

 Case 2: when width is 100um

 ![100u](https://github.com/user-attachments/assets/e7d6c5e8-9042-43b1-8771-a629b2959f0c)


 Inference: in case 1 and 2 we can observe that i hve doubled the width of the channel so crrespondingly the is increase in the case 2 because as width of the channel increases the number of charges flowing through the channel also increases so due to increase in widths so current also increases.
 

 AC Analysis:

 ![ac1](https://github.com/user-attachments/assets/bb3d24dd-9a0c-44a9-9a90-9218c14f67cd)
 

 ![ac2](https://github.com/user-attachments/assets/60360546-f4c2-46c3-908d-f3ee1b2903bb)


 Transient analysis:

 



 




 
 

     
     
     



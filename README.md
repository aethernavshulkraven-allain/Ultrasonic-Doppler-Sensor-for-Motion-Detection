# SonarProject

# Objective
The objective of the lab assignments – over the course of the semester – is to learn how to
(a) Design
(b) Simulate
(c) Fabricate and
(d) Test a narrowband ultrasonic Doppler sensor for motion detection.
# Skills Gained
(a) Learn how to read a datasheet and choose appropriate components for a design
(b) Learn how to draw a schematic
(c) Learn how to simulate the behavior of the circuit on LTSpice
(d) Do the PCB layout required for fabrication
(e) Solder components on the PCB
(f) Test the performance of the circuit and compare the performance with simulation results

# Description
The system level configuration of the ultrasonic narrow band Doppler sensor is shown in Figure.1. The
system consists of transmitter and receiver circuits. The transmitter consists of a crystal oscillator that
generates a 2MHz sinusoidal signal. The frequency divider divides the 2MHz signal by a factor of 50 to generate a 40KHz (fo) output signal. A low pass filter is used to remove any higher order harmonics that
may be generated. The filter may be designed as an active filter to provide voltage amplification to the
transmitted signal. The signal may be amplified and conveyed to the acoustic transducer where the
electrical signal is converted to acoustic signal and transmitted as shown in the equation below.

![image](https://github.com/aethernavshulkraven-allain/Ultrasonic-Doppler-Sensor-for-Motion-Detection/assets/112583472/a4f0aad5-9ce7-48d7-b1bd-8dcffba5c09f)


The received signal from a moving target consists of a Doppler shifted signal.

![image](https://github.com/aethernavshulkraven-allain/Ultrasonic-Doppler-Sensor-for-Motion-Detection/assets/112583472/ef8a01bc-daaa-4551-a1ef-d0eed64e1667)


The received signal is much weaker than the transmitted signal (Arx < Atx). Hence, the signal is passed
through a low noise amplifier for voltage amplification. Then the signal is band pass filtered to remove
higher order harmonics and limit external interference. The signal is then captured in the oscilloscope. The
frequency domain of the received signal should show a shift in the frequency from 40KHz when a target
moves before the sonar. Note that when the hand is moving, the Doppler frequency shift may change with
time. Note that the sonar must be configured such that the strong transmitted signal does not directly leak
into the receiver. The transducers are typically very directional. So the sonar must be carefully configured
such that the transmitter and receiving transducers do not face each other and instead face the target.
While performing experiments with a moving target, please ensure that the target is within the field of view
of the sonar.


![image](https://github.com/aethernavshulkraven-allain/Ultrasonic-Doppler-Sensor-for-Motion-Detection/assets/112583472/fc2e5367-63f1-46cd-a4d6-95de4cda4edc)

![image](https://github.com/aethernavshulkraven-allain/Ultrasonic-Doppler-Sensor-for-Motion-Detection/assets/112583472/528abcad-afdb-4374-adc5-05096acd3d2a)


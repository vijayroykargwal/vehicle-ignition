# vehicle-ignition
I’ve done pcb design on CADSTAR11.1 because cadsoft eagle not available at this time. I’ve used PIC16F877P micro-controller which works as-
1.	Micro-controller should turn on an LED1 on pressing a button.
2.	Should be able to sense voltage from a noisy 12V external source(like a vehicle’s ignition status) and turn on LED2
 
Things which is used in pcb design:-
1.	2 layer 1.6mm PCB
2.	Power supply as 5v vcc & other noisy  12v external source(car’s battery or vehical’s ignition status)
3.	When I’ll give less than 5v to MC using 10k ohm resister in series with 5v vcc,it runs.
4.	I’ve programmed to MC microc code in keil software and run in proteus pro 8 as-
First there is a 12v to 5v convertor.A transitor configured as an emitter follower has a very high impedence at the collecter.the high impedence is going to block the noise.we can use here a VOLTAGE DIVIDER CIRCUIT but the noise can’t be removed. Now this 5v goes to ADC pin (RA0/AN0).this voltage sense by the MC & LED2 is turn on. Where a simple LED1 turn on using simple 5v vcc of MC when switch (x2) is turn on.
5.component specification is given below as attached pdf file.
6.Track width- vcc-15.0,GND-20.0, signal-10.0
7.copper plate width &length given in default pcb circuit.

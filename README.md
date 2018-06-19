## Welcome to Imperial Department of Physics!!!

Hi, welcome to Blackett Laboratory!! This is the website of our summer project,

**DIY Heartbeat Monitor**

[editor on GitHub](https://github.com/Plankat/heartbeat.github.com/edit/master/index.md) 

[Jekyll](https://jekyllrb.com/) 

### Introduction


This heart-rate monitor is a simple infrared heartbeat monitor.  By shining an infrared LED through the thumb to a photodiode, the change in the intensity of infrared can be detected and shown on an oscilloscope after amplification. The number of change in the signal is counted and displayed as average heart rate. 





### Background


We used an infrared light as the light source, the light will penetrate the finger and reach the photodiode detector on the other side. When heart contracts and pumps blood, the pressure in the arteries will change therefore change the blood density and the diameter of capillaries. Then the reflection of the light causes a change in the intensity of the light received by the photodiode, and subsequently resulted in a change in potential. The signal is then being processed by the circuit and finally show on the oscilloscope. The rate of heartbeat is then counted and shown on the LCD screen. 


-Circuit Diagram
![.](C:\Users\Plank\Desktop\Lab3\2.png)

-Practical Circuit
![.](C:\Users\Plank\Desktop\Lab3\5.png)


-Sample Pulse Oscillograph
![.](C:\Users\Plank\Desktop\Lab3\3.png)
![.](C:\Users\Plank\Desktop\Lab3\4.png)






### In Greater Detail...

1. High pass filter
A high-pass filter (HPF) is an electronic filter that passes signals with a frequency higher than a certain cut-off frequency and attenuates signals with frequencies lower than the cut-off frequency. This HPF consists of a resistor and capacitor, and the potential difference at either side of the resistor is the output. 



2. Amplifier
An amplifier is used to increase the power of a signal. The amount of amplification provided by an amplifier is measured by its gain: the ratio of output voltage to the input voltage. In this circuit we used non-inverting amplifier, and the gain can be calculated by following formula: 
Gain=1+R/(R_ground) 
Here the total gain for the first op-amp amplifier is 561 The second is 101. Note that the capacitor connected here is used for smoothing the signal.


3. Low pass filter
A low-pass filter (LPF) is a filter that passes signals with a frequency lower than a certain cut-off frequency and attenuates signals with frequencies higher than the cut-off frequency. A low-pass filter is the complement of a high-pass filter. It is also consists of a resistor and a capacitor but arranged in a different way. The output of this LPF is the potential difference across the capacitor.


4. Peak Detector
A peak detector is a series connection of diode and capacitor outputting a DC voltage that is equal to the peak value of the input AC signal. The real voltage output is lower since there is a voltage drop across diode.

5. Comparator
A comparator is a device that compares two input digital or analog signals and output a signal indicating which is larger. 
![Fig 1](https://en.wikipedia.org/wiki/Comparator#/media/File:Opamp105.gif)
When Vin>Vref ,Vout=high. When Vin<Vref, Vout=low 

6. Microcontroller
A microcontroller is a complicated integrated circuit which is used in automatically controlled devices such as remote controls. A microcontroller contains one or more CPUs (processor cores) along with memory and programmable input/output peripherals. In this project, we use Arduino Uno.   

7. LCD
Liquid-crystal display, often know as LCD, is a flat-panel display or other electronically modulated optical device that uses the light-modulating properties of liquid crystals. Liquid crystals do not emit light directly, instead using a backlight or reflector to produce images in color or monochrome.





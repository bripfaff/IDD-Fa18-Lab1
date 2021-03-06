# IDD-Fa18-Lab1: Blink!

**A lab report by Brian Pfaff**

<!--- **Fork** this repository to get a template for Lab 1 for *Developing and Designing Interactive Devices* at Cornell Tech, Fall 2018. You should modify this `README.md` file to delete this paragraph and update below. As the lab asks:--->


<!--- > Include your responses to the bold questions on your own fork of the lab activities. Include snippets of code that explain what you did. Deliverables are due next Tuesday. Post your lab reports as `README.md` pages on your GitHub, and post a link to that on your main class hub page.--->

<!---We've copied the questions from the lab here. Answer them below!
--->

## Part A. Set Up a Breadboard

https://github.com/bripfaff/IDD-Fa18-Lab1/blob/master/41072576_499850473814502_1370875972298997760_n.jpg


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**

Brown Black Brown

**b. What do you have to do to light your LED?**

I only had to press the installed button for the LED to light up. The green light on top of the LED was on when I plugged in the arduino board and so I did notneed to do anything for that. 

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

https://youtu.be/EBD9TK4xvCQ

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**

Did not need to change any lines of code to make the LED blink

**b. What line(s) of code do you need to change to change the rate of blinking?**

The number in the delay() function 

**c. What circuit element would you want to add to protect the board and external LED?**

 A Resistor so that a minimum resistance is in the circuit. This makes sure that all the current isn't forced into the LED at once according to Ohm's Law (I= V/R)
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**

When I set the delay function to delay(10) I cannot percieve that it is blinking any longer. To prove to myself that it is infact still blinking, I changed The delay at the end of the loop so that the time between blinks was increased and now i can percieve the very fast blink that occurs due to the delay between the turning off of the LED and the restating of the loop. 

**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**

https://github.com/bripfaff/IDD-Fa18-Lab1/blob/master/My-blink-lab1

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

https://youtu.be/xME1D10-KTc


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**

Yes, The LED did glow the who turning of the potentiometer. The glow was very low on one end of the spectrum and seemed not to increase very much for the first few degrees of turning however after the halfway point, the LED started glowing stronger and stronger as the dial turned towards the end that went to ground. 

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

I need to take out the potentiometer and add a wire from port 11 to the LED curciut so that there is a close curcuit connected to a por thtat supports PWM in arduino. In terms of the code, just had to make sure that the correct port was being called when the code was intialized 

**b. What is analogWrite()? How is that different than digitalWrite()?**

AnalogWrite is used to send specific value of frequency through a PWM capable pin in the arduino board. This is different to DigitalWrite as digitalwrite only has two states (high voltage-on, low voltage-off) where as analogwrite can have several states

** Arduino Sketch **
https://github.com/bripfaff/IDD-Fa18-Lab1/blob/master/my_fade_lab1

## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

https://github.com/bripfaff/IDD-Fa18-Lab1/blob/master/40684467_1378916132211707_2721058564532600832_n.jpg

Inside the device there are 5 resistors, a processor and an LED. 

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

Yes, there is a processor in the mouse. The processor is in the centre of the mother board. It is processing how the light is changing as the mouse moves over a surface. This is then converted in that processor so that the computer can understand how to deal with the changes in the light flow. I believe that the 4 resistors on the mouse have something to do with this in terms of determining direction through flow of current.

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

Yes, there is a sensor that detects changes in light reflection as a mouse flows over the surface. As stated above, I believe that the  4 resistors in the mouse have something to do with how the sensed information is conveyed to other portions of the device. 

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

The device is power by a usb point. This is then connected to the board as indicated below. 

**d. Is information stored in your device? Where? How?**

No, I don't think that information is stored on it. 

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**

There are two easily accessable wires on the LEd that can used to hijack the LED. This makes it a very easy hack due to the accessability of the wires. The only precaution is that I add a resistor to the curcuit for the safety of the LED. 

### 3. Build your light!

**Make a video showing off your Frankenlight.**
https://youtu.be/a8-69snQAWU
**Include any schematics or photos in your lab write-up.**

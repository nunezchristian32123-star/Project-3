# Project-3
Example of PWM with an LED
PIN 3 is the only used PIN in this project
delay d is set to 5 to allow fast cycling between upscaling and descaling duty cycles
in the first for loop int a is set to 0 with condition a<256 if true a scales up by one (a++)
delay d is then applied
analogWrite writes a to the output of pin three allowing for the PWM duty cycle to scale from low to high in this case changing its brightness from low to high
Condition runs until duty cycle is 100% (a=255)
another for loop is added to turn the brightness down with near same conditions
int a is set to 255 (Max or 100% duty cycle) with condition a>=0 and if confition a-- if true.
analogWrite writes the duty cycle a to pin 3 in this case going from 100% to 0% duty cycle
delay is then set between analogWrite or descaling duty cycles
this turns down the brightness of the led.

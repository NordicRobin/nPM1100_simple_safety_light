The nPM1100 simple safety light is a concept sketch for using the nPM1100's "ship mode" as the on/off switch for a 
rechargeable bicycle light or other small flashlight. This gives it the simple button-press activation we're used to from 
this type of device, without the need for a microcontroller. \
\
Many rechargeable bicycle lights [needs citation] use some sort of microcontroller to control the charging and on/off functionality, 
as well as different blinking modes of the LEDs on the bicycle lights. In my experience, these microcontrollers tend to drain 
the battery of the light when left unused for a period of time. By using the nPM1100's ship mode
as a power-down mode, the light consumes only 0.45 uA while powered off. This would also be the case if a microcontroller was included in the design, as the 
nPM1100 ship mode cuts power to all devices it's powering while in this mode. \
\
As an extra challenge, the nPM1100's inputs for entering and exiting ship mode have opposite polarities, therefore a simple PNP bipolar junction transistor (BJT) is included to 
flip the polarity of the button press, when the BJT is powered by the nPM1100's regulator. The BJT adds to the current consumption of the light while the circuit is powered on, 
but does not affect the 0.45 uA current draw of the system while in ship mode. 

![image](https://github.com/NordicRobin/nPM1100_simple_safety_light/assets/48379998/a62d27e2-494f-49f5-9d2d-1e94c82a2af6)

# Panasonic_NN-S235WF_microwave_oven  
hack and build the controller.  
it is US$100 kitchen tools and became a toy once malfuction, why so easy broken tools?  


MN101C78A, mask rom MCU, no way to replace or repair this microwave oven as controller broad malfunctioning suddently.  
Panasonic build the MCU and matsushita manufacturing, later nvuoton brand named.  
see datasheet [IC_datasheet](IC_datasheet)  

### user manual  
[user manual, service manual etc. pretty much useless, not for component level of trouble shooting](manual)  

### symtom  
LCD has no display, power supply and 18V is good, on-broad 3.3V is good, 8MHz xtal is good, reset circuit is good. so the only problem came to be fault of this MCU.  
![photo/6.jpg](photo/6.jpg)  


### circuit diagram of the oven  
![photo/panasonic_NN-S235WF_schenmatic.jpg](photo/panasonic_NN-S235WF_schenmatic.jpg)  


### to understand how this microwave oven regulated the power
ON-OFF control for transformer to power magnetron, that the esential of regulated the power of microwave oven (old model without uses of inverter design)  
![photo/power_level_control_microwave_oven.JPG](photo/power_level_control_microwave_oven.JPG)  


### power_broad  
the 18V supply, relays and buzzer  
complete project log, [power_broad](power_broad)
![power_broad/power_broad_pcb3.jpg](power_broad/power_broad_pcb3.jpg)



### controller PCB
![photo/controller3.jpg](photo/controller3.jpg)  


### why the SHORT SWITCH (or Monitor SWITCH) and why fuse burn  
[see tranining and why manual](manual)  
![photo/short_switch_adjustment.JPG](photo/short_switch_adjustment.JPG)  



### to build my own controller ?
this is no much more than a "timer" + relays to control for the microwave oevn, the following is reference, and perhaps good however the license was saying no any publish could be allowed as saying with an opensource code & project ?  
https://extremeelectronics.co.in/avr-projects/microwave-controller-using-atmega8-avr-project/  

another github hosted open source project that seems promising,  
https://github.com/SamuelGold/arduino-microwave-oven  


### try arduino and open source code  
LCD1602, a few button and code, it is easy, ON-OFF control and timer setting would be only barrier for the project. let us see what would be.

### last time membrane fault, key press and repair by cleaning
complete project log, [panel_fix](panel_fix)  
![panel_fix/panel_contact.jpg](panel_fix/panel_contact.jpg)  

### last time plate motor fix by glue
complete project log, [plate_motor_fix](plate_motor_fix)   
![plate_motor_fix/4.jpg](plate_motor_fix/4.jpg)   


### video log for microwave oven and energy control
turns out that simple on/off control to power the magnetron, heat spreading and function of time is only way to control the heating level.  
this is true for all kinds of non-invertor design of microwave oven.  

https://www.facebook.com/laba.xiao.75/videos/6765868633453997/

### removed short-swtich  
bad design & unreliability of door lock mechanism, the fault of fuse burn or MCB tripped
there is no way to re-design such door lock linkage or the swtich fastenning, simplest way is to remove the short switch to ensure no fues burn upon door open/close, the major drawback was that omitted safety protection for door opening when microwaving. User has own resiponsible to stop power before open the door.   
![photo/microwave_oven_removed_short_switch.png](photo/microwave_oven_removed_short_switch.png)


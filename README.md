# Panasonic_NN-S235WF_microwave_oven
hack and build the controller


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


### controller PCB
![photo/controller3.jpg](photo/controller3.jpg)  


### why the SHORT SWITCH and why fuse burn  
[see tranining and why manual](manual)  
![photo/short_switch_adjustment.JPG](photo/short_switch_adjustment.JPG)  


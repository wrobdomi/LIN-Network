# LIN-Network
Automotive network simulation. 
This project simulates working of air conditioning system in a car vehicle. The project was developed with use of CANoe software. 

## What is LIN ?
In a nutshell, LIN network is a communication bus used in vehicles to exchange data. In comparison to CAN bus, LIN costs less and is low speed.  This bus can be usful for applications that are not time-critical such as air conditioning system. 

# Automatic air-coditiong system

## Working principle of the project : 
The system works in accordance to the principle of working of LIN network. There is master node which is a control unit and two
slaves - temperature sensor and windows opening sensor. The air conditiong system must be switched on by one of the passangers. After that, the system is active only if all windows remain closed.  
Passanger can set desired temperature inside vehicle. System compares temperature set by passanger and  temperature inside and it sets air conditionig on a proper level of working. If difference between these temperatures is greater than 5, than system is cooling or heating air on level 2. If less than five than level 1. If no difference, than it stops cooling / heating.  
Topology view :   
![lin1](https://user-images.githubusercontent.com/37666186/38031173-e640762e-329a-11e8-8df4-c7e7793e18b4.PNG)

## GUI 
To simulate and test the system, GUI was developed. GUI cen be controlled by clicking switches on the air conditioning panel and by pressing keyboard buttons as follows :
- Set temperature outside '-' or '+' change temperature one degree up or down.
- '1' and '2' switches on and off automatic air conditiong system. 
- 's' and 'a' to simulate that any window is open or all widnows are closed
- red arrow and blue arrow on the ritgh of a panel, to set desired temperature inside vehicle
- blue or orange arrow ont the left of a panel indicates wheather system is cooling or heating air  
![lin2](https://user-images.githubusercontent.com/37666186/38032004-e34d8806-329c-11e8-9375-b2cf4b6b12e3.PNG)
![wdwadwa](https://user-images.githubusercontent.com/37666186/38033524-83690704-32a0-11e8-879d-c9f40c2a70ca.gif)


## Another features
The system has diagnostics and error handling features. One of them is polling slaves by a master before starting transfer data ( diagnostic frames ). To visualize this process LEDs are lighted when positive response is received. Also 'trace' windows enable looking at frames.   
![aaaaaa](https://user-images.githubusercontent.com/37666186/38032690-90d59f76-329e-11e8-8712-11615d2d5d22.gif)  
![der](https://user-images.githubusercontent.com/37666186/38033171-b68db194-329f-11e8-80ad-0428506dc754.gif)


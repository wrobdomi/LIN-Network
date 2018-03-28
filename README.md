# LIN-Network
Automotive network simulation. 
This project simulates working of air conditioning system in a car vehicle. The project was developed with use of CANoe software. 

## What is LIN ?
In a nutshell, LIN network is a communication bus used in vehicles to exchange data. In comparison to CAN bus, LIN costs less and is low speed.  This bus can be usful for applications that are not time-critical such as air conditioning system. 

## Working principle of the project : 
The system works in accordance to the principle of working of LIN network. There is master node which is a control unit and two
slaves - temperature sensor and windows opening sensor. The air conditiong system must be switched on by one of the passangers. After that, the system is active only if all windows remain closed. 
Passanger can set desired temperature inside vehicle. System compares temperature outside and inside and it sets air conditionig on a proper level of working. If difference between these temperatures is greater than 5, than system is cooling or heating air on level 2. If less than five than level 1. If no difference, than it stops cooling / heating. 
Topology view : 


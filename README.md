# TVC-rocket-simulation-using-MATLAB


## Intuition behind the model

MATLAB Simulink is a versatile software for simulation of various dynamic systems. The goal of my project was to accurately simulate a model Thrust Vectored Controlled (TVC) rocket and apply a PID control loop to get level stable flight. The model uses basic Simulink libraries along with the 3 Degree of freedom (3DOF) aerospace blockset which is the back bone of the entire simulation. 

A TVC rocket maintains it's stable flight by changing the angle of thrust vector mount in the X and Z (In this case) to maintain stable flight. The 

## Breaking down the model

### Thrust block
This block deals with the input to the system, here the input the system is assumed to be ideal constant thrust. The direction of the rocket’s magnitude vector is resolved into its vertical and horizontal vectors and then multiplied with the average thrust and feed into the 3DOF block, to simulate the force which acts on the moment arm the Center of mass values is also added.

### 3DOF Block


### PID Control block and Lag

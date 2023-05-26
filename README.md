

---

# DC Motor Dynamics Simulation Project

## Overview

This project aims to understand and illustrate the dynamics of a Direct Current (DC) motor by leveraging the principles of physics and mathematics. Through a series of differential equations that model the motor's behavior, we're able to capture the motor's response to varying voltage inputs over time.

The simulation uses basic physical parameters of a DC motor, such as armature resistance, armature inductance, back-emf constant, torque constant, rotor inertia, and rotor damping. The chosen parameters are used to describe a typical DC motor, but these can be modified to emulate different motor specifications.

![image](https://github.com/Minato0859/Mathematical-Modelling-of-a-DC-Motor/assets/123880338/f5dd2fb0-8232-440f-abf0-12b41636b792)


One of the significant features of this project is its capability to generate a graphical representation of the relationship between the applied voltage and the motor's terminal angular velocity at t=1s. This characteristic helps us understand the influence of voltage on the motor's performance, demonstrating the motor's behavior under different operating conditions.

![image](https://github.com/Minato0859/Mathematical-Modelling-of-a-DC-Motor/assets/123880338/0498bc42-6647-4616-8484-1ca5cf1f81ce)


## Implementation Details

This project is implemented using Python, with the aid of scientific libraries such as NumPy, SciPy, and Matplotlib. The `solve_ivp` function from the SciPy library is used for solving the ordinary differential equations, while Matplotlib is used to visualize the motor's behavior.

## How to Run the Project

To run this project, ensure you have Python installed, along with the following Python libraries: NumPy, SciPy, and Matplotlib. These can be installed using pip:

```bash
pip install numpy scipy matplotlib
```

After the required libraries are installed, execute the script using Python:

```bash
python motor_dynamics_simulation.py
```

This will generate plots displaying the motor's angular velocity and current over time, as well as the relationship between the voltage applied and the terminal angular velocity at t=1s.

## Code Example

The script is divided into sections defining motor parameters, implementing the motor dynamics function, setting initial conditions, determining the time span for the simulation, solving the ODEs, and finally plotting the results.

Here's a sneak peek into the code structure:

```python
import numpy as np
from scipy.integrate import solve_ivp
import matplotlib.pyplot as plt

# Motor parameters
R = 8.57  # Ohm, armature resistance
L = 0.1692  # H, armature inductance
...
```

## Glimpse at other key graphs

### Figure 1.4 setting the damping to 0.00004 N*m/(rad/s)

![image](https://github.com/Minato0859/Mathematical-Modelling-of-a-DC-Motor/assets/123880338/76b19704-6f66-4016-8bf1-5e3f9b379b56)

### Figures 2.00-2.99 (100 graphs of varied voltages) 

![image](https://github.com/Minato0859/Mathematical-Modelling-of-a-DC-Motor/assets/123880338/f450873a-2fc3-4a29-ad29-819249ef0e2e)



## Future Work

The current implementation offers a simplified representation of a DC motor's behavior. For future enhancements, it can be extended to incorporate more complex situations like fault modeling, thermal effects, or the introduction of different control strategies for manipulating the motor's speed or torque.

---



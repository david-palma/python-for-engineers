# Unmanned Aerial Vehicle (UAV) swarm dynamic coordination and control

This exercise focuses on the coordination and control of a swarm of drones to form various geometric formations while ensuring collision avoidance and minimising energy consumption. The study involves system modelling, control strategy implementation, simulation, and visualisation, providing practical experience in multi-agent systems and control theory. The coordination of drone swarms has applications in fields such as search and rescue, environmental monitoring, and surveillance, requiring synchronised movement, collision avoidance, and energy-efficient operation. The simulation models the swarm aligning into dynamic geometric shapes, including a star, hexagon, square, circle, and triangle, with a focus on implementing control strategies and optimising swarm behaviour.

## Objectives

The primary objectives of this exercise are:

1. **Swarm coordination**:
   Develop algorithms to coordinate the movement of multiple drones to form specific geometric shapes while ensuring uniform distribution within the specified region.

2. **Collision avoidance**:
   Implement mechanisms to ensure that drones avoid collisions while moving towards the desired formation.

3. **Energy optimisation**:
   Minimise the energy consumption of the drones during the alignment process.

4. **Dynamic formation change**:
   Simulate the drones changing their formation dynamically every few seconds to a different geometric shape.

5. **Comparison of control strategies**:
   Implement and compare the effectiveness of Proportional-Integral-Derivative (PID) Control and Linear Quadratic Regulator (LQR) in guiding the drones to their target positions.

## Methodology

The methodology for this exercise is structured into the following stages:

1. **System model formulation**:
   Model the dynamics of individual drones, including their position, velocity, and control inputs. Define the target positions for the geometric shapes: star, hexagon, square, circle, and triangle.

2. **Control strategy and collision avoidance**:
   Implement control strategies for each drone to move towards its target position using PID and LQR control. Integrate collision avoidance mechanisms to ensure safe navigation.

3. **Simulation and visualisation**:
   Simulate the behaviour of the drone swarm under various conditions and visualise the swarm's movement and formation using Python libraries, including Matplotlib and Matplotlib Animation.

4. **Dynamic formation change**:
   Implement a mechanism to dynamically change the target formation every few seconds, cycling through the different geometric shapes.

5. **Comparison of control strategies**:
   Compare the effectiveness of PID and LQR control strategies in terms of energy consumption, collision avoidance, and accuracy in achieving the desired formations.

## Testing the system

The exercise includes several test scenarios to validate the system and explore its behaviour under varying conditions:

1. **Formation test**:
   Implement the control algorithm to achieve the desired geometric formation without obstacles, ensuring uniform distribution of drones.

2. **Collision avoidance test**:
   Integrate obstacle detection and avoidance, and evaluate the swarm's ability to avoid collisions while forming the geometry.

3. **Energy optimisation test**:
   Compare the energy consumption of PID and LQR control strategies in achieving the formation.

4. **Dynamic formation change test**:
   Simulate the dynamic change of formations every few seconds and evaluate the swarm's ability to adapt to new target positions seamlessly.

---

This exercise provides a hands-on opportunity to explore the principles and techniques of coordinating and controlling drone swarms. It is particularly relevant for engineers and researchers involved in the development of multi-agent systems, focusing on the integration of control algorithms, collision avoidance, and energy optimisation in a dynamic environment.

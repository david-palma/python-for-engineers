# Simulation of tornado dynamics and their impact on building structures using Navier-Stokes equations

This exercise explores the dynamic behaviour of tornadoes and their impact on building structures, with an emphasis on fluid flow patterns and the resulting structural stress and damage. Tornadoes are complex, highly destructive atmospheric vortices that pose significant risks to buildings and infrastructure. The analysis involves simulating the wind field generated by a tornado using the two-dimensional incompressible Navier-Stokes equations, identifying regions of high velocity and pressure, and assessing the structural response to these forces. The study employs a simplified two-dimensional model, such as a standardised building cross-section, to balance computational efficiency and accuracy. This approach is relevant to fields such as civil engineering, meteorology, and disaster risk management, where understanding and mitigating tornado impacts are critical concerns.

## Objectives

The primary objectives of this exercise are:

1. **Wind field simulation**: Model and visualise the two-dimensional wind field generated by a tornado, focusing on the variations in wind velocity and pressure over time and space.

2. **Structural stress assessment**: Evaluate the stress distribution within the building structure caused by the tornado-induced wind forces, identifying regions susceptible to structural damage or failure.

3. **Risk evaluation**: Assess the risk of structural damage based on the wind velocity and pressure profiles. This includes determining whether the building's structural integrity is compromised under extreme wind conditions.

## Methodology

The methodology follows these structured steps:

1. **Initial and boundary conditions**: Define the building structure and surrounding environment with known material properties and geometric dimensions. Specify the initial conditions of the wind field, representing the tornado. Boundary conditions account for wind interactions with the building and the surrounding environment.

2. **Navier-Stokes equations**: Solve the two-dimensional incompressible Navier-Stokes equations to model the fluid dynamics of the tornado wind field. This includes accounting for air viscosity, density, and pressure variations.

3. **Numerical simulation**: Implement a numerical method, such as finite difference or finite element analysis, to compute the wind velocity and pressure distribution across the building structure over time.

4. **Visualisation and analysis**: Generate wind velocity and pressure plots over time to visualise the impact of the tornado on the building. Assess the resulting structural stress to identify regions prone to damage or failure.

## Testing the system

The exercise includes several test scenarios to validate the system and explore its behaviour under varying conditions:

1. **Uniform building test**: A simulation is conducted on a uniform building structure with standardised material properties. This test assesses the basic wind field interaction and ensures that the solution conforms to expected fluid dynamics behaviour.

2. **Heterogeneous building test**: A second simulation introduces variability in material properties and structural features, such as openings and reinforcements. This test evaluates the model's robustness in handling diverse building structures.

3. **Environmental condition test**: Adjust environmental conditions, such as wind speed and direction, to simulate varying tornado characteristics. This test validates the system's flexibility in adapting to different tornado scenarios.

4. **Custom configuration test**: Input custom building properties, tornado intensity, and environmental conditions to explore different scenarios and their impact on structural stress and damage.

---

This exercise demonstrates the application of numerical modelling to solve a real-world problem, combining principles of fluid dynamics, structural engineering, and disaster risk management to address the challenges posed by extreme weather events.

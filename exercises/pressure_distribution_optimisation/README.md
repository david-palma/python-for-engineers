# Simulation and optimisation of pressure distribution in a combustion chamber

This exercise focuses on the simulation and optimisation of pressure distribution within a combustion chamber to ensure efficient fuel combustion and enhance engine performance. The design and optimisation of pressure distribution are crucial for achieving a uniform distribution, and this analysis involves simulating how various burner configurations affect the pressure distribution. The study uses a two-dimensional model that balances computational efficiency with accuracy, making it applicable to various engineering fields where combustion efficiency is critical.

## Objectives

The primary objectives of this exercise are:

1. **Pressure distribution simulation**: Simulate and visualise the pressure distribution within a combustion chamber with variable geometry.

2. **Geometric variation effects**: Evaluate the impact of geometric variations on the pressure distribution within the chamber.

3. **Configuration optimisation**: Optimise the configuration of the combustion chamber to achieve an optimal pressure distribution.

## Methodology

The methodology follows these structured steps:

1. **Initial and boundary conditions**: Define the combustion chamber as a two-dimensional domain in the $\left(x, y\right)$ space. The Poisson equation will be used to model the pressure distribution:

   - $P\left(x, y\right)$ is the pressure at position $\left(x, y\right)$.
   - $f\left(x, y\right)$ is the pressure source distribution due to the burners.
   - $k$ is a proportionality constant, assumed to be 1 for simplicity.

2. **Source function definition**: Model the source function $f(x, y)$ as a sum of Gaussian functions centred at the burners' positions:

    $$ f(x, y) = \sum_{i=1}^N A_i \exp{\left(-\frac{\left(x - x_i\right)^2 + \left(y - y_i\right)2}{\sigma^2}\right)} $$

    - $\left(x_i, y_i\right)$ are the coordinates of the $i$-th burner.
    - $A_i$ is the intensity of the $i$-th burner, assumed to be 1 for all $i$.
    - $\sigma$ is the variance parameter of the $i$-th burner.

3. **Numerical simulation**: Implement the Poisson equation to simulate the pressure distribution. Use numerical methods, such as the finite difference method, to solve the equation.

4. **Visualisation and analysis**: Generate pressure distribution plots to visualise the effect of geometric variations. Assess the pressure distribution to identify regions with suboptimal pressure gradients.

5. **Optimisation**: Optimise the burner positions and intensities to achieve a uniform pressure distribution. Use optimisation techniques, such as gradient descent, to find the optimal configuration.

## Testing the system

The exercise includes several test scenarios to validate the system and explore its behaviour under varying conditions:

1. **Uniform geometry test**: Conduct a simulation with a standardised combustion chamber geometry to verify the basic pressure distribution.

2. **Variable geometry test**: Introduce geometric variations to evaluate the system's robustness in handling different configurations.

3. **Optimisation test**: Test the effectiveness of the optimisation algorithm in achieving a uniform pressure distribution.

4. **Custom configuration test**: Input custom burner positions, intensities, and geometric configurations to explore their impact on pressure distribution.

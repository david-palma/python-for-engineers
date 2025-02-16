# SIR model for the diffusion of an infectious disease with vaccination and quarantine

This exercise explores the diffusion of an infectious disease within a population using an extended SIR (Susceptible, Infected, Removed) model that incorporates vaccination and quarantine. By simulating disease spread across five compartments—Susceptible (S), Infected (I), Removed (R), Vaccinated (V), and Quarantined (Q)—the study evaluates the effectiveness of intervention strategies in mitigating outbreaks. The analysis involves solving a system of differential equations governing the transitions between compartments, providing a more comprehensive representation of disease control measures. Using Python a specific library, the numerical solutions are visualised through time-series plots and heat maps, offering insights into the impact of vaccination coverage and quarantine efficacy on disease dynamics.

## Objectives

The primary goals of this exercise are as follows:

1. **Disease diffusion analysis**: Simulate the spread of an infectious disease within a population and observe how it evolves over time under different scenarios.

2. **Control measure evaluation**:

    - Assess the impact of vaccination rates on reducing the susceptible population and limiting disease spread.
    - Analyse the effect of quarantine in isolating infected individuals and slowing transmission.

3. **Numerical solution**: Solve the extended SIR model using the `scipy` library to compute the temporal dynamics of the compartments.

4. **Data visualisation**:
    - Generate time-series graphs to illustrate the evolution of each compartment (S, I, R, V, Q) over time.
    - Use heat maps to demonstrate the effectiveness of vaccination and quarantine strategies under varying parameters.

## Methodology

The methodology employed in this study consists of the following steps:

1. **Model definition**:

    - Extend the classical SIR model by introducing additional compartments:
        - **Vaccinated (V)**: Represents individuals who are immunised and cannot contract or transmit the disease.
        - **Quarantined (Q)**: Represents infected individuals who are isolated to prevent further transmission.
    - Define the differential equations governing the transitions between these compartments based on key parameters, including infection rate, recovery rate, vaccination rate, and quarantine rate.

2. **Parameter selection**:

    - Set baseline values for model parameters such as population size, initial conditions, and rates of infection, recovery, vaccination, and quarantine.
    - Define scenarios to explore the impact of varying vaccination and quarantine rates.

3. **Numerical simulation**:

    - Use the `scipy.integrate.odeint` function to solve the system of differential equations for each scenario.
    - Compute the time-dependent behaviour of all compartments.

4. **Data visualisation**:
    - Plot time-series graphs to depict the evolution of the compartments over time.
    - Create heat maps to illustrate how different combinations of vaccination and quarantine rates affect key metrics, such as peak infection levels and total infections.

## Testing the system

The exercise includes several test scenarios to validate the system and explore its behaviour under varying conditions:

1. **Baseline scenario**: Simulate the disease diffusion with no vaccination or quarantine, serving as a reference for evaluating the effectiveness of interventions.

2. **Vaccination impact**: Analyse scenarios with varying vaccination rates to determine the threshold coverage required to achieve herd immunity and significantly reduce infections.

3. **Quarantine efficacy**: Explore the effect of different quarantine rates on controlling the spread, focusing on reducing the peak number of infections and total outbreak duration.

4. **Combined measures**: Test the combined impact of vaccination and quarantine, identifying optimal strategies for minimising the disease spread under resource constraints.

---

This exercise demonstrates the application of mathematical modelling and numerical simulation in understanding infectious disease dynamics. By integrating vaccination and quarantine into the SIR framework, the analysis provides valuable insights into the design of effective public health interventions. The results underscore the importance of timely and coordinated control measures in mitigating the impact of infectious diseases on populations.

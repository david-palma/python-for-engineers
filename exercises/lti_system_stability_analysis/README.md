# Analysis of the stability of an LTI dynamic system: a mass-spring-damper model

This exercise investigates the stability of a linear time-invariant (LTI) dynamic system, specifically a mass-spring-damper system, by evaluating the eigenvalues of its state-space representation. The stability of LTI systems is a key topic in engineering, with applications in control theory and mechanical systems. The system's stability is analysed through time-domain plots and eigenvalue diagrams, with various system parameters, such as mass, damping coefficient, and spring constant, being varied to observe their impact on the system's stability.

## Objectives

The primary objectives of this exercise are:

1. **Modelling the mass-spring-damper system**:
    - Develop a state-space representation of the mass-spring-damper system.
    - Derive the system's state matrix using parameters such as mass, damping coefficient, and spring constant.

2. **Stability analysis**:
    - Compute the eigenvalues of the state matrix to assess system stability.
    - Determine the system’s stability based on the real parts of the eigenvalues, with negative real parts indicating stability and positive real parts suggesting instability.

3. **Parameter sensitivity**:
    - Investigate how variations in system parameters (e.g., mass, damping coefficient, and spring constant) influence the eigenvalues and the overall stability of the system.

4. **Visualisation and interpretation of results**:
    - Simulate the time-domain response of the system for different parameter values and plot the displacement and velocity of the mass.
    - Visualise the system’s eigenvalues in the complex plane to illustrate stability conditions.

## Methodology

The analysis follows these structured steps:

1. **State-space representation**
    - Derive the state-space equations for the mass-spring-damper system, which describe the system in terms of its state variables (displacement and velocity).
    - The state-space system is given by:
      $$\dot{x}(t) = Ax(t) + Bu(t)$$
      $$y(t) = Cx(t) + Du(t)$$
      where $A$ is the state matrix, $B$ is the input matrix, $C$ is the output matrix, and $D$ is the feedthrough matrix.

2. **Eigenvalue analysis**:
    - Compute the eigenvalues of the state matrix to determine the system's stability. Eigenvalues with negative real parts indicate stability, while those with positive real parts suggest instability.

3. **Parameter variation**:
    - Vary the  system's physical parameters (mass $m$, damping coefficient $c$, and spring constant $k$) and compute the eigenvalues for each parameter set.
    - Observe how the location of the eigenvalues changes with varying parameters, particularly focusing on different damping conditions.

4. **Damping scenarios**:
    - Critically damped: Achieved when the damping coefficient is set such that the system returns to equilibrium as quickly as possible without oscillating. The system’s eigenvalues will have negative real parts with no imaginary components.
    - Overdamped: Occurs when the damping coefficient is higher than the critical damping value, causing the system to return to equilibrium slowly without oscillating. The eigenvalues are negative with larger real parts compared to the critically damped case.
    - Underdamped: This happens when the damping coefficient is too low, causing the system to oscillate before settling at equilibrium. The eigenvalues have negative real parts with non-zero imaginary components.

5. **Simulation and visualisation**:
    - Simulate the system’s response over time for different sets of parameters corresponding to critically damped, overdamped, and underdamped configurations.
    - Plot the time-domain response (displacement and velocity of the mass) for each damping scenario.
    - Generate eigenvalue plots in the complex plane to visualise the stability conditions based on the location of the eigenvalues relative to the imaginary axis.

## Testing the system

The system is tested under a variety of configurations to evaluate its stability across different damping conditions:

1. **Baseline test**: Simulate the system with default parameter values (mass, damping, spring constant) and validate results using the eigenvalue analysis.
2. **Critically damped test**: Set the damping coefficient to the critical value for each mass and spring constant configuration, and observe the system’s response. Verify that the system does not oscillate and returns to equilibrium without overshooting.
3. **Overdamped test**: Increase the damping coefficient beyond the critical value and observe the system’s slower return to equilibrium. Note the larger real parts of the eigenvalues.
4. **Underdamped test**: Decrease the damping coefficient below the critical value and examine the system’s oscillatory response before reaching equilibrium. The eigenvalues should show negative real parts with non-zero imaginary components.
5. **Custom parameter test**: Allow for custom input of mass, damping, and spring constant values to explore different configurations and their effects on system stability.
6. **Visualisation**:
    - Time-domain response plots: Illustrate the displacement and velocity of the mass over time for each damping condition, highlighting oscillatory, critically damped, and overdamped behaviours.
    - Eigenvalue plots: Display the eigenvalues in the complex plane for each test case, showing how the stability of the system changes with variations in damping.

---

This exercise highlights the fundamental principles of stability analysis in LTI systems. By systematically varying system parameters and observing the effects on stability across different damping scenarios (critically damped, overdamped, and underdamped), users can intuitively understand how the physical properties of the system influence its stability. The insights from this study are widely applicable to control engineering and dynamic modelling.

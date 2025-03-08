# Python for Engineers

This repository contains a curated collection of exercises from the **"Python for Engineers"** course at the University of Udine, taught by [**Prof. David Palma**](https://david-palma.github.io/). The materials focus on practical problem-solving, with an emphasis on applying Python programming to address various engineering challenges. These exercises are designed to foster hands-on experience in solving real-world engineering problems using computational methods.

## Overview

The repository includes a range of exercises, varying in complexity and scope, to provide a comprehensive learning experience:

- **Foundational Exercises**: These simpler tasks introduce basic concepts, providing the foundation for solving engineering problems using Python. They are ideal for those seeking to gain familiarity with Python's role in engineering contexts.

- **Advanced Exercises**: These more complex problems require a deeper understanding of engineering principles and focus on solving specific, real-world engineering challenges by applying advanced computational techniques.

The exercises span a wide range of engineering disciplines, including mechanics, thermodynamics, control systems, signal processing, and more. The primary objective is to leverage Python to solve practical engineering problems, with an emphasis on the following areas:

- **Data analysis and manipulation**
- **Data visualisation**
- **Numerical simulations**
- **Mathematical modelling**
- **Signal processing**
- **Control systems design**

Each exercise includes a Jupyter Notebook that demonstrates the entire problem-solving process. The notebooks contain data analysis, computational methods, and visualisation of results. Users are encouraged to follow each notebook step-by-step to understand the methodology used and replicate the findings.

## Exercises

The repository currently includes the following exercises:

1. [**Advanced modelling of projectile motion**](exercises/projectile_motion_simulation/)\
    This exercise models projectile motion under ideal and realistic conditions, considering air resistance and variable gravity. It aims to compare trajectories, range, and maximum height using numerical solutions, highlighting the effects of environmental factors on motion.

2. [**Automated wear analysis of a gear**](exercises/gear_wear_analysis/)\
    This exercise explores the automated analysis of a gear's wear by examining its teeth. The focus is on detecting wear patterns that can impact the gear's performance and longevity, using computational methods to identify and quantify damage based on geometric features.

3. [**Analysis of the stability of an LTI dynamic system**](exercises/lti_system_stability_analysis/)\
    This exercise analyses a mechanical system’s stability and dynamic response by varying mass, damping, and stiffness. It explores underdamped, critically damped, overdamped, and stable systems, calculating eigenvalues and simulating displacement and velocity over time.

4. [**Analysis of the thermal effects of a lightning strike on a structural element**](exercises/thermal_analysis/)\
    This exercise analyses the thermal effects of a lightning strike on a structural element, focusing on heat distribution, temperature gradients, and fire/structural damage risks. It uses numerical modelling to simulate heat propagation and assess material failure under extreme thermal conditions.

5. [**SIR model for the diffusion of an infectious disease with vaccination and quarantine**](exercises/infectious_disease_spread/)\
    This exercise models the spread of an infectious disease within a population, incorporating vaccination and quarantine as intervention measures. It explores how varying vaccination and quarantine rates affect the dynamics of infection, recovery, and mortality, providing insights into optimal strategies for controlling disease outbreaks through numerical simulations of the SIR model.

6. [**Simulation and optimisation of pressure distribution in a combustion chamber**](exercises/pressure_distribution_optimisation/)\
    This exercise focuses on simulating and optimising the pressure distribution within a combustion chamber to ensure efficient fuel combustion and enhance engine performance. The study involves analysing various burner configurations, visualising pressure distribution, and optimising burner positions and intensities using numerical methods.

7. [**Unmanned Aerial Vehicle (UAV) swarm dynamic coordination and control**](exercises/drone_swarm_coordination/)\
    This exercise examines the dynamic coordination and control of UAV swarms to form various geometric formations, ensuring collision avoidance and minimised energy consumption. It involves system modelling, linearisation, and state-space representation. A comparative analysis of LQR and PID control strategies is conducted, evaluating performance based on stability, accuracy, and efficiency to determine the most effective approach for UAV swarm coordination.

8. [**Simulation of tornado dynamics and their impact on building structures using Navier-Stokes equations**](exercises/tornado_dynamics_simulation/)\
    This exercise explores the dynamic behaviour of tornadoes and their impact on building structures, focusing on fluid flow patterns and the resulting structural stress and damage. It involves simulating the wind field generated by a tornado using the two-dimensional incompressible Navier-Stokes equations, identifying regions of high velocity and pressure, and assessing the structural response to these forces.

---

### How to Run the Exercises

The exercises in this repository are provided as Jupyter Notebooks. To run the notebooks and replicate the results, follow the steps below:

#### 1. Launch Jupyter Notebook

Start the Jupyter Notebook server by executing:

```bash
jupyter notebook
```

A browser window should open automatically, displaying the Jupyter interface. Navigate to the folder containing the desired exercise (e.g., `exercises/` ) and select the corresponding notebook to open.

#### 2. Execute the Notebook

Once the notebook opens:

- Read the introductory section to understand the context of the case study.
- Execute the cells sequentially to reproduce the results and visualisations.

For detailed instructions on setting up your environment and installing dependencies, refer to the [Installation Guide](docs/installation.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

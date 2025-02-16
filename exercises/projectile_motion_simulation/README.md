# Advanced modelling of projectile motion

This exercise explores the two-dimensional motion of a projectile under both ideal and realistic conditions, incorporating trajectory analysis with factors such as air resistance and variable gravitational acceleration. Projectile motion is a fundamental concept in physics and engineering, providing insight into motion under the influence of gravity and external forces. This study extends the traditional model by introducing realistic effects, enhancing understanding of kinematic principles and numerical modelling techniques.

## Objectives

The primary objectives of this exercise are:

1. **Fundamental modelling**:
    - Develop a mathematical representation of projectile motion under ideal conditions (constant gravity, no air resistance).
    - Derive analytical expressions for trajectory characteristics, including range and maximum height.

2. **Extend the model to include realistic conditions**:
    - Integrate velocity-dependent drag forces to simulate air resistance.
    - Model gravitational acceleration as a function of altitude to simulate motion over large vertical distances.

3. **Numerical analysis and solution**:
    - Solve the system of coupled differential equations describing the motion using numerical integration techniques.
    - Compare analytical solutions with numerical results to evaluate model accuracy.

4. **Visualisation and interpretation of results**:
    - Create trajectory plots to illustrate differences between ideal and advanced models.
    - Analyse the impact of environmental factors and initial conditions on motion.

## Methodology

The analysis follows these structured steps:

1. **Ideal conditions**

    - Use the basic kinematic equations to model the motion:
      $$x(t) = v_0 \cos(\theta)t$$
      $$y(t) = v_0 \sin(\theta)t - \frac{1}{2}gt^2$$
    - Derive analytical formulas for time of flight, maximum height, and range.
    - Simulate and plot the trajectory under ideal conditions.

2. **Motion with air resistance**

    - Incorporate drag force
      $$F_d = -kv$$
    - Formulate the equations of motion:
      $$\frac{dx}{dt} = v_x, \quad \frac{dy}{dt} = v_y$$
      $$\frac{dv_x}{dt} = -\frac{k}{m}v_x, \quad \frac{dv_y}{dt} = -g - \frac{k}{m}v_y$$
    - Solve numerically using methods such as Runge-Kutta or Euler’s method.
    - Analyse the reduction in range and maximum height due to drag.

3. **Motion with variable gravity**

    - Model gravitational acceleration as:
      $$g(y) = g_0 \left( \frac{R}{R + y} \right)^2$$
      where $R$ is Earth’s radius.
    - Update and solve the equations of motion to study the effects of variable gravity.

## Testing the system

The system is tested under a variety of scenarios to evaluate its accuracy and adaptability:

1. **Baseline test**: Simulate ideal motion and validate results using analytical solutions.

2. **Air resistance test**: Explore the effect of different drag coefficients on the trajectory.

3. **Variable gravity test**: Simulate motion for projectiles reaching significant altitudes, examining how variable gravity alters the trajectory.

4. **Parameter sensitivity test**: Investigate how variations in $v_0$ and $\theta$ affect key metrics such as range and maximum height.

5. **Visualisation**:

    - **Trajectory plots**: Display the path of the projectile under ideal and advanced conditions.
    - **Parameter influence plots**: Show how initial conditions and environmental factors impact key metrics.
    - **Comparative plots**: Overlay ideal and advanced trajectories to emphasise the role of drag and variable gravity.

---

This exercise offers a comprehensive exploration of projectile motion, blending theoretical principles with practical simulation. By extending the classical model, students gain advanced insights into the effects of environmental factors and numerical modelling techniques, making this analysis directly applicable to real-world engineering and physics problems.

# DeepONet for Dynamics Mechanical Systems

This project investigates the use of Deep Operator Networks (DeepONet) for learning the solution operator of dynamical systems governed by ordinary differential equations.

## Physical Problem

The considered system is a single-degree-of-freedom mechanical system governed by

$$
m\ddot{x}(t)+c\dot{x}(t)+kx(t)=f(t)
$$

where:

- $m$ : mass
- $c$ : damping coefficient
- $k$ : stiffness
- $f(t)$ : external force

## Objective

The objective is to learn the nonlinear operator

$$
G:f(t)\rightarrow x(t)
$$

That mapping an input force signal to the corresponding displacement response.

## Workflow

1. Generate training data using numerical integration by SciPy's.
2. Train a DeepONet model.
3. Predict unseen dynamical responses.
4. Compare predictions against numerical solutions.

## Repository Structure

```text
notebooks/
src/
figures/
results/
```

## Future Extensions

- Multi-degree-of-freedom systems
- Bearing dynamics
- Gear dynamics
- Physics-informed DeepONet
- Digital twins

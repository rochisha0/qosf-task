# Submission of Task 2 and Task 3 for the screening of QOSF Mentorship Program

## Task 2

I have used `pennylane` with `qiskit` library plugin to solve the screening task. 

#### The steps involved in the solution:

* Creating a parametrized circuit using RX and RY and CNOTs for creating `|01>` and `|10>` with eaual probability and and running it on a noisy simulator.
  * Applied a parametrized RY gate and RX gate on first and second qubit respectively and measured the probability of the states.
* Started with chosing random parameters.
* Created a cost function which returns `((prob_00-0)**2 + (prob_01-0.5)**2 + (prob_10-0.5)**2 + (prob_11-0)**2)` where `prob_x` gives the probability of the given state
* Used a prebuilt `Gradient Descent Optimizer` in `pennylane` library to find the parameters for different number of measurements.
* Plotted the state probability for different number of measurements.

#### Steps involved in the bonus question:

* I measured the expectation value of `X@X` for the state, where `@` is the `tensor product`.
* Then minimized `-1*expectation value` to find the parameter using `Gradient Descent`

## Task 3

I have used `qiskit` library to solve the Task 3. 

#### The steps involved in the solution

* Created `H`, `X`, `Y`, `Z`, `CNOT` gate using `RX`, `RZ`, `CZ`.
* Reduced the overhead by `Basic Swap`.

## Note

If you want to evaluate with only one task, please go ahead with **Task2**.

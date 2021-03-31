# Data-driven distributionally robust MPC using the Wasserstein metric

This project contains the experimental framework for distributionally robust MPC and two case studies, per "Data-driven distributionally robust MPC using the Wasserstein metric" by Zhengang Zhong, Ehecatl Antonio del Rio-Chanona and Panagiotis Petsagkourakis, submitted to IEEE CDC 2021.

## Abstract

Distributionally robust optimization is a technique for decision making under uncertainty where the probability distribution of the uncertain problem is itself subject to uncertainty. A novel data-driven MPC scheme is proposed to control constrained stochastic linear systems using distributionally robust optimization. Distributionally robust constraints based on Wasserstein ball are imposed to bound the expected state constraint violation in the presence of process disturbance. A feedback control law is solved to guarantee that the predicted states comply with constraints with regard to the worst-case distribution within the Wasserstein ball centered at the discrete empirical probability distribution. The resulting distributionally robust MPC framework is tractable and efficient. The effectiveness of the proposed scheme is demonstrated through two numerical case studies.

## How to Run Experiments

``python inverted_pendulum.py `` or ``python mass_spring.py`` to run the simulation for one realization.

``python`` other file_name to execute simulations for multiple realizations.



## Simulation results

### Simulation 1: 50 realizations of the data collection algorithm for a mass spring system initialized with different numbers of samples

![PDF1](https://github.com/OptiMaL-PSE-Lab/CDC2021/blob/master/fig/fig1.png) {width=75%}

<img src="https://github.com/OptiMaL-PSE-Lab/CDC2021/blob/master/fig/fig1.png" width="40%">

The shaded area denotes the 25-th to 75-th trajectory distribution.

### Simulation 2: Mass spring system averaged from 50 realizations with sample number ranging from 1 to 10

![PDF2](https://github.com/OptiMaL-PSE-Lab/CDC2021/blob/master/fig/fig2.png){width=75%}

### Simulation 3: Relation between sample number and constraint violations within first four seconds in simulation 2

![PDF3](https://github.com/OptiMaL-PSE-Lab/CDC2021/blob/master/fig/fig3.png){width=75%}

### Simulation 4: Inverted pendulum system averaged from 10 realizations with Wasserstein ball radius ranging from 0.01 to 100

![PDF4](https://github.com/OptiMaL-PSE-Lab/CDC2021/blob/master/fig/fig4.png){width=75%}

### Simulation 5: Relation between Wasserstein ball radius and constraint violations within first two seconds in simulation 4

![PDF5](https://github.com/OptiMaL-PSE-Lab/CDC2021/blob/master/fig/fig5.png){width=75%}


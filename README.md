# Performative Prediction in a Stateful World

## Abstract
Deployed supervised machine learning models make predictions that interact with and influence the world. This phenomenon is called *performative prediction* by Perdomo et al. (ICML 2020). It is an ongoing challenge to understand the influence of such predictions as well as design tools so as to control that influence. We propose a theoretical framework where the response of a target population to the deployed classifier is modeled as a function of the classifier and the current state (distribution) of the population. We show necessary and sufficient conditions for convergence to an equilibrium point of two retraining algorithms, *repeated risk minimization* and a lazier variant. Furthermore, convergence is near an optimal classifier. We thus generalize results of Perdomo et al.,~whose performativity framework does not assume any dependence on the state of the target population. A particular phenomenon captured by our model is that of distinct groups that acquire information and resources at different rates to be able to respond to the latest deployed classifier. We study this phenomenon theoretically and empirically. 
## Code

This repository contains the experiments we run to investigate performative prediction in a stateful world. Particularly, we used the setting of *strategic classification* in load application. The code is based on the [`whynot`](https://github.com/zykls/whynot) Python package, and it is an adaptation of the [`dynamic_decisions`](https://github.com/zykls/whynot/tree/master/examples/dynamic_decisions) examples.

There are two notebooks:

1. `performative_prediction.ipynb` - Replication of Perdomo et al. simulation.
1. `performative_prediction-groups-respond-slowly.ipynb` - 3 Groups Respond Slowly setting.

### Setup (in the command line)

1. Install Pipenv (Instructions [here](https://pipenv.pypa.io/))
1. Clone this repository `git clone https://github.com/shlomihod/performative-prediction-stateful-world-review.git`
1. `cd performative-prediction-stateful-world`
1. `pipenv install`
1. `jupyter notebook`

# Performative Prediction in a Stateful World

### Gavin Brown, Shlomi Hod, Iden Kalemaj


## Abstract
Deployed supervised machine learning models make predictions that interact with and influence the world. This phenomenon is called \emph{performative prediction} by Perdomo et al. (2020), who investigated it in a stateless setting. We generalize their results to a world with a state, in which the response of the population to the deployed classifier depends both on the classifier and the previous distribution of the population. We also explore such a setting empirically, for the scenario of strategic manipulation.

## Code

This repository contains the experiments we run to investigate performative prediction in a stateful world. Particularly, we used the setting of *strategic classification* in load application. The code is based on the [`whynot`](https://github.com/zykls/whynot) Python package, and it is an adaptation of the [`dynamic_decisions`](https://github.com/zykls/whynot/tree/master/examples/dynamic_decisions) examples.

There are four notebooks:

1. [`performative_prediction.ipynb`](https://github.com/gavinrbrown1/algsocproject/blob/master/performative_prediction.ipynb) - Replication of Perdomo et al. simulation
1. [`performative_prediction-groups-respond-slowly.ipynb`](https://github.com/gavinrbrown1/algsocproject/blob/master/performative_prediction-groups-respond-slowly.ipynb) - Three-groups respond slowly setting.
1. [`performative_prediction-decay.ipynb`](https://github.com/gavinrbrown1/algsocproject/blob/master/performative_prediction-decay.ipynb) - Geometric decay response.

### Setup (in the command line)

1. Install Pipenv (Instructions [here](https://pipenv.pypa.io/))
1. Clone this repository `git clone https://github.com/shlomihod/performative-prediction-stateful-world.git`
1. `cd performative-prediction-stateful-world`
1. `pipenv install`
1. `jupyter notebook`
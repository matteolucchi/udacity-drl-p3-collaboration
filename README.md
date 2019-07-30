# Project 2: Continuous Control - Udacity DRL Nanodegree
Implementation of a Deep Reinforcement Learning agent to solve the Unity Tennis environment.

This repository contains all the material relative to the implementation of the Project 3 of the [Udacity Deep Reinforcement Learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) program.


## The Environment
The environment consists of two agents that control tennis rackets. The goal of each agent is to keep the ball in play.

<!--  Insert GIF of env-->
<!-- ![tennis](url) -->

The following description is for each of the two agents
### State Space
- **Size:** 8

- **Content:** Position and Velocity of the ball and the racket

### Action Space
- **Size**: 2

- **Actions:** Movement towards (or away from) the net, Jumping

### Reward

- **+0.1**  : if an agents hits the ball over the net
- **-0.01** : if an agent lets a ball hit the ground or hits the ball out of bounds

### Goal

The environment is considered solved when the average of the maximum score between the two agents over 100 consecutive episodes is greater than *+0.5*.

## Installation

Follow the instructions below to install the software necessary to run the agent in the environment.

**1.** Set up the Python environment on your machine by following the [instructions in the DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies).

**2.** Download the Unity environment:
- [Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- [Mac OSX](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- [Windows 32-bit](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- [Windows 64-bit](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

**3.** Place the unzipped folder just downloaded in the `p3_collab-compet/` folder in the DRLND GitHub repository.

**4.** Clone [this repository](https://github.com/matteolucchi/udacity-drl-p3-collaboration) in the `p3_collab-compet/` folder in the DRLND GitHub repository.

## How to run the code

The agent can be tested and trained in the [Tennis.ipynp](https://github.com/matteolucchi/udacity-drl-p1-navigation/blob/master/Tennis.ipynb) python notebook. Following the instructions in the notebook it is possible to see our trained agent in action or to train a new agent using the hyperparameters of your choice and to see your agent in action.

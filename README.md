[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation

### Introduction

For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

### Project Files

`model.py` - PyTorch model of the Q Network

`agent.py` - DQN agent

`Navigation.ipynb` - Jupyter notebook with training and visualization code

`checkpoint.pth` - Final saved PyTorch checkpoint

### Getting Started

Install dependencies by running `pip install -r requirements.txt`.

Run or modify the learning process with `jupyter notebook` -> `Navigation.ipynb`.

Enabling variants:
* Double DQN - set `doubleQ=True` when initializing `Agent`
* Dueling DQN - set `dueling=True` when initializing `Agent`
* Prioritized Experience Replay - set `per=True` when initializing `Agent`

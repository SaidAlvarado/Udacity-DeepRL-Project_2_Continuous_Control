# Udacity's Deep RL Nanodegree - Project 1: Navigation

[//]: # (Image References)

[image2]: https://user-images.githubusercontent.com/10624937/42386929-76f671f0-8106-11e8-9376-f17da2ae852e.png "Kernel"


## Introduction

This repository contains my solution for the first project of the Deep Reinforcement Learning Nanodegree from Udacity. In this exercise an RL-agent is dropped into a large square environment where it must collect yellow bananas scattered around the world while avoiding the blue ones. The environment was made with Unity's ML-Agents framework. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/11748427/80967527-cc864e00-8e16-11ea-8467-df71ffbbeb5b.gif" alt="Trained Agent"/>
</p>


## Environment Definition

#### Rewards

- Each **yellow** banana collected provides a reward of **+1**.
- Each **blue** banana collected provides a reward of **-1**.
- No rewards are provided in a per-time-step basis.

#### State Space

The state space has 37 dimensions and consists of the agent's velocity, as well as ray-based perception of objects in front of the agent.

#### Action Space

The agent has four discrete actions available at it's disposal:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

#### Task Goal

The agent must learn to select the appropriate action to maximize the amount of yellow bananas it collects in each episode of the task. In order to consider the environment solved, the agent must get an average score of +13 over 100 consecutive episodes.



## Getting Started

Most of these instructions were borrowed from the instalation instructions in Udacity's [Deep Reinforcement Learning Repository](https://github.com/udacity/deep-reinforcement-learning).


### Prepare the Anaconda Environment


1. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name drlnd python=3.6
	source activate drlnd
	```
	- __Windows__: 
	```bash
	conda create --name drlnd python=3.6 
	activate drlnd
	```

2. Clone the repository (if you haven't already!), and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/SaidAlvarado/Udacity-DeepRL-Project_1_Navigation.git
cd Udacity-DeepRL-Project_1_Navigation/python
pip install .
```

3. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.  
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

4. Before running code in the notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu. 

![Kernel][image2]

### Download the Unity Environment


5. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

6. Decompress the file into the root directory of the repository.

### Run the code.

7. Follow the instructions in `Navigation.ipynb` to train and see the agent in action.


## Understanding the Algorithm

For more information regarding the algorithm used to solve this environment, please refer the the technical report `Report.md` included in the repository.


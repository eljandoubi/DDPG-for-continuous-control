[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"
[image3]: https://user-images.githubusercontent.com/10624937/42386929-76f671f0-8106-11e8-9376-f17da2ae852e.png


# DDPG for continuous control
This repository contains material from the [second Udacity DRL procjet](https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control) and the coding exercice [DDPG-pendulum](https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum).


## Introduction

In this project, I trained a DDPG agent to solve two types of environment.  

![Trained Agent][image1]

First the **Reacher** environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

---
Second, the **Crawler** environment.

![Crawler][image2]

In this continuous control environment, the goal is to teach a creature with four legs to walk forward without falling. 

___
An environment is considered solved, when an average score of +30 over 100 consecutive episodes, and over all agents is obtained. 

## Dependencies

To set up your python environment to run the code in this repository, follow the instructions below.

1. Create (and activate) a new environment with Python 3.9.

	- __Linux__ or __Mac__: 
	```bash 
    conda create --name drlnd 
    source activate drlnd
	```
	- __Windows__: 
	```bash
	conda create --name drlnd 
	activate drlnd
	```
2. Follow the instructions in [Pytorch](https://pytorch.org/) web page to install pytorch and its dependencies (PIL, numpy,...). For Windows and cuda 11.6

    ```bash
    conda install pytorch torchvision torchaudio cudatoolkit=11.6 -c pytorch -c conda-forge
    ```
	

3. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.  
	- Install the **box2d** environment group by following the instructions [here](https://github.com/openai/gym#box2d).

    ```bash
    pip install gym[box2d]
    ```
    
4. Follow the instructions in [second Udacity DRL procjet](https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control) to get the environment.
	
5. Clone the repository, and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/eljandoubi/DDPG-for-continuous-control.git
cd DDPG-for-continuous-control/python
pip install .
```

6. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.  
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

7. Before running code in a notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu. 

![Kernel][image3]

## Training and inference
You can train and/or inference an environment by following instructions in its notebook.

## Implementation and Resultats

The implementation and resultats are discussed in the report.

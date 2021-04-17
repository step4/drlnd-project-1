# Project: Navigation
*Embrace your inner gorilla!*

## Introduction
In this project, we want to train an agent, a gorilla if you like, who only loves yellow bananas and hates the blue ones.

For that he will learn to naviagte in a large, square Unity World:

![gorilla](images/gorilla.gif)

In the manner of Deep-Q-Learning the agent will be rewarded with a +1 for collecting a yellow banana and with a -1 for each blue banana.  
So in easy words: **Collect all yellow and avoid all blue bananas!**

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, our agent must get an average score of atleast +13 over 100 consecutive episodes.

We will use a improved Double DQN approach such that our target average score will be +16 over 100 consecutive episodes.
## Get started
First of all: Make sure you run this repository on a 64-bit Windows 10 machine and have anaconda, miniconda, etc. installed!

If all requisites are met run the following lines one by one in your terminal of choice:

```bash
conda create -n drl-p-1 python=3.6
conda activate drl-p-1
conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch
cd ./python
pip install .
```

After that we can use pytorch to train our agent and all necessary packages to use a given Unity Environment to see our *gorilla* in action.

## Train and run the agent
To train and see the trained agent in action. Just open the `Navigation.ipynb` Notebook in Jupyter and let all cells run.
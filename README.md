# Foraging_DRL_Project

This is the group project of Group 1 of the course CS698R **Deep Reinforcement Learning** which explores the performance of various RL agents on a patch foraging environment. Our problem focuses on solitary foraging. We are trying to answer how an animal feeding on a particular food patch, and hence depleting it, decides when it is optimal to leave the patch in search of a richer one, provided that it has only a finite amount of time to forage in that environment. An example rendering of one of the variants of the given environment for our problem can be seen through this link: https://youtu.be/qRH_PKusOIw <br>

We have implemented various conventional RL algorithms and deep RL algorithms to solve the given problem which is specified below.<br>

The code implementation for **Multi Arm Bandit** is in the `MAB_agents.ipynb` notebook. The notebook implements the problem as a multi arm bandit problem where each arm represents the number of times each patch must be harvested before the agent moves on to the next patch.<br>

The code implementation for **Control Agents** is in the `ControlAgents.ipynb` notebook. The notebook implements various control agents on the environment to obtain optimal results.<br>

The code implementation for **Control Agents** is in the `Rich_Patch_Poor_Patch.ipynb` notebook. The notebook implements various control agents on the tich patch poor patch environment with variable intitial rewards.<br>

The code implementation for **Deep Learning Agents** is in the `deep_agents_foraging-v0.ipynb` and `deep_agents_foraging-v1.ipynb` notebook. The `deep_agents_foraging-v0.ipynb` notebook implements **DQN**, **DDQN** and **VPG** on the linear patch with constant initial reward. The `deep_agents_foraging-v1.ipynb` notebook implements **DQN**, **DDQN** and **VPG** on the linear patch with rich and poor patches which have different initial rewards.<br>



The environment is in the dir `gym-env/gym_env/envs/.`

There are five Environments, each for:
- Foraging with constant initial reward for tabular method.
- Foraging with variable initial reward for tabular method.
- Foraging with constant initial reward for deep learning method with revised state space.
- Foraging with varible initial reward for deep learning method with revised state space.
- A demo environment with visual rendering
 

## To install the gym environment, run:
```
git clone git@github.com:Exploration-Lab/CS698R-Project-Patch-Leaving-Decisions-1
cd gym-env
pip install -e .
```

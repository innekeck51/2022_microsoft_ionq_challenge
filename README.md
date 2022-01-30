# Classical vs Quantum World Agent on Snake Game Using IonQ-Qiskit

## Personal experience
The project team consists of myself, I am Inneke Cynthia Kusumawardhani, from Indonesia. I love quantum information science

![](/img/AnimatedGames.gif)
Ilustration Agent on Snake Game

## Concept
Reinforcement Learning (RL) is a simple idea to grasp. Interaction with the environment is how an agent learns. The agent chooses an action and receives feedback in the form of states (or observations) from the environment and rewards. This cycle will continue indefinitely or until the agent ends in a terminal state. 
During an episode, the agent's purpose is to maximize the sum of the rewards. The agent does a lot of exploring at the start of the learning phase: it tries different actions in the same state. It need this information in order to determine the best course of action for the states. Exploration reduces as learning progresses. Instead, the agent will take advantage of his actions: this means he will choose the action that maximizes the reward, based on his experience.
Snake game implementation with it. The objective is to collect as many foods as possible while avoiding colliding with a wall or the snake's body.

## Outline of the Project
The project is divided into two phases: the first RL that uses classical environtment, Q Learning method. In the second phase running into environtment Quantum (Quantum World) using qiskit and ionQ provider.

More in detail, in this repository you find two codes:

1. **Classical World**
We implemented Q learning (RL), Snake.py is a snake game build with python. QLearning.py learning process for agent to play the snake game using Q-Learning. The game will provide you a reward for each move the snake make. There is a negative reward if the snake collides with itself or a wall. There is a positive reward if the snake advances towards the food. Initially, the Q matrix is filled with zeros. The Q table is updated after each move made by the agent.

2. **Quantum World**
Quantum Reinforcement Learning with parameterized quantum circuit (PQCs), using OpenAI Gym, and Cart Pole [[1]](#1). In this project, agent in quantum world analysed running on ioq provider, and simulator.
### IonQ-simulator
<img src="./img/IonQ-simulator.png" alt="IonQ-Simulator" width="300px">
### IonQ-qpu
<img src="./img/IonQ-qpu.png" alt="IonQ-QPU" width="300px">

## Requirements
Packages are used in this code:

* `Qiskit` 
* `Qiskit Machine Learning`
* `PyTorch`
* `gym`
* `numpy` , `matplotlib`


## Reference
<a id="1">[1]</a>  Andrea Skolik, Sofiene Jerbi, Vedran Dunjko (2021), _Quantum agents in the Gym: a variational quantum algorithm for deep Q-learning_, [arXiv:2103.15084](https://arxiv.org/abs/2103.15084).


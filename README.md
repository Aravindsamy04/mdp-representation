# MDP REPRESENTATION

## AIM:
The goal is to make traffic flow better. By using smart decisions for traffic lights and other actions.

## PROBLEM STATEMENT:

### Problem Description
In this traffic managing project, the goal is to optimize the flow of traffic in a given road network using Markov Decision Process (MDP) and Reinforcement Learning techniques. 

### State Space
The state space includes current traffic status at intersections, vehicle count on roads, traffic light colors, and environment factors like weather. It's like gathering puzzle pieces for making traffic smoother.

### Sample State
A sample state could include the number of vehicles waiting at each intersection, the current signal state at each intersection, and the congestion levels on different roads.

### Action Space
The action space holds choices for traffic control: changing signal colors, timing adjustments, and even redirecting vehicles.

### Sample Action
An example of an action could be changing the traffic signals from red to green at a specific intersection, allowing traffic to flow in a certain direction.

### Reward Function
The reward function is designed to provide feedback to the reinforcement learning agent on how well it's performing.

##### Smooth flow of traffic without sudden stops or traffic jams
##### Efficient utilization of road capacity
##### Minimization of delays for vehicles

### Graphical Representation:
![111](https://github.com/Aravindsamy04/mdp-representation/assets/113497037/28d2cfff-5c33-4341-85d1-de5077deff5c)

## PYTHON REPRESENTATION:
```python
pip install git+https://github.com/mimoralea/gym-walk#egg=gym-walk

import gym
import gym_walk

P ={
    0: {
        0: [(1.0, 0, 0.0, True), (0.0, 0, 0.0, True), (0.0, 0, 0.0, True)],
        1: [(1.0, 0, 0.0, True), (0.0, 0, 0.0, True), (0.0, 0, 0.0, True)]
    },
    1: {
        0: [(1.0, 0, 0.0, True), (0.0, 1, 0.0, False), (0.0, 2, 1.0, True)],
        1: [(1.0, 2, 1.0, True), (0.0, 1, 0.0, False), (0.0, 0, 0.0, True)]
    },
    2: {
        0: [(1.0, 2, 0.0, True), (0.0, 2, 0.0, True), (0.0, 2, 0.0, True)],
        1: [(1.0, 2, 0.0, True), (0.0, 2, 0.0, True), (0.0, 2, 0.0, True)]
    }
}
```
## OUTPUT:

![1](https://github.com/Aravindsamy04/mdp-representation/assets/113497037/bdc73868-6054-4483-ae51-f5ca899a995b)


## RESULT:
Thus, the MDP is used to create a smart traffic management approach to reduced congestion and shorter travel times. 

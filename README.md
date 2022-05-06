# Deep Reinforcement Learning Nanodegree

This repository contains my **Deep Reinforcement Learning** solution to one of 
the stated problems within the scope of the following Nanodegree:

[Deep Reinforcement Learning Nanodegree Program - Become a Deep Reinforcement Learning Expert](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893)



Deep Reinforcement Learning is a thriving field in AI with lots of practical 
applications. It consists of the use of Deep Learning techniques to be able to
solve a given task by taking actions in an environment, in order to achieve a 
certain goal. This is not only useful to train an AI agent so as to play videogames, 
but also to set up and solve any environment related to any domain. In particular, 
as a Civil Engineer, my main area of interest is the **AEC field** (Architecture, 
Engineering & Construction).

## Collaboration and Competition Project

This project consists of a Collaboration and Competition problem, which is contained within the Policy 
Based Methods chapter and is solved by means of a Deep Deterministic Policy Gradient algorithm (DDPG).

### Environment description

The environment used for this project is based on the *Unity ML-Agents* Tennis 
environment from 2018. There is no clear equivalent in 2022, but the closest would be the
[Soccer Environment](https://github.com/Unity-Technologies/ml-agents/blob/main/docs/Learning-Environment-Examples.md#soccer-twos).

It consists of a tennis playground, in which there is a racket-shaped agent at each side of the net. The agents can 
move around in order to be able to bounce the ball over the net to the other side of the playground. The goal for the 
agents is to keep the ball in play for as many time steps as possible.

![alt text](https://user-images.githubusercontent.com/10624937/42135623-e770e354-7d12-11e8-998d-29fc74429ca2.gif)
<br/>

Its characteristics are as follows:
- The state space consists of 8 variables corresponding to the position and velocity of the ball and racket.
- The action space consists of 2 continuous actions, corresponding to movement perpendicular to the net, and jumping.
- An agent receives a reward of +0.1 when it is able to hit the ball over the net. On the contrary, if it lets the ball 
touch the ground or hit it out of bounds, it receives a reward of -0.01.

### Getting Started

Firstly, the reader is advised to set up the 
[Soccer Environment](https://github.com/Unity-Technologies/ml-agents/blob/main/docs/Learning-Environment-Examples.md#soccer-twos)
instead of the legacy Tennis one, specially if not following the Nanodegree. This will allow to install recent 
versions of the libraries and potentially avoid some unfixed bugs from old versions.

#### Installing required dependencies

Having said that, the exact environment used in this repository -for the scope of the Nanodegree- can be setup by
following the instructions from the "Dependencies" header on the link below, which becomes *Step 1*:
[udacity/deep-reinforcement-learning](https://github.com/udacity/deep-reinforcement-learning#dependencies)

As *Step 2*, the compressed file corresponding to the user operating system must be downloaded from one of the links 
below, and placed inside the `./p3_collab-compet/` folder after unzipping it.
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

At this point, *Step 3* requires to clone the current repository and place the folder at the root of the freshly 
configured *deep-reinforcement-learning*. From there, it only remains to change the environment path(s) to match the 
file(s) downloaded in *Step 2*. This path can be changed at 
[the following line of environment.py](https://github.com/cvillagrasa/DeepReinforcementLearning_Navigation/blob/c3b8224bd47d720f740136269a0f198f5f20c1f9/environment.py#L12).

Lastly, *Step 4* consists of installing Seaborn within the Python environment by running `pip install seaborn`.

And that's it. After those four steps, the Jupyter Notebook *Continuous_Control.ipynb* from this repository can already 
be executed.

### Solution

My solution to the posed problem can be found in the 
[Solution Report](https://htmlpreview.github.io/?https://github.com/cvillagrasa/DeepReinforcementLearning_Navigation/blob/master/Report.html), 
as well as in the code included 
within this repository.

It is worth stating that it has been a fascinating exercise which has let me further understand the implications of 
multi-agent training in a challenging environment with sparse rewards.

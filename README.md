# UAV_ENVIRONMENT
UAV_ENVIRONMENT_DEEP_Q_LEARNING
Create your own UAV environment with the following requirements:
Assume that we have a UAV environment:
      + Area: 2000 x 2000 (m)
      + The step of UAV: around 30-50 (m) for each step (you can define by yourself)
      + Users: be static and follow a Gaussian distribution
      + UAV’s coverage: 400 (m)
      + Objective: Maximize the number of users supported by the UAV’s coverage
Let’s define the Action, Reward, and State for the environment:
   - Action: Up, down, left, right, and remain stationary (5 actions - discrete actions)
   - Reward: Consider Nt the number of users supported by the UAV’s coverage at step t:
      + If Nt+1 > Nt: Reward = 1
      + If Nt+1 < Nt: Reward = -1
      + If Nt+1 = Nt: Reward = 0
Required RL Algorithm: DQN model

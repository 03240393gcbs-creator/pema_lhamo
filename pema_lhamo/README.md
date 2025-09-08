1.  What type of space is the action space? How many actions are there?
 The action space is Discrete(2). This means there are 2 possible actions: 0 (push the cart left) and 1 (push the cart right).

2.  What type of space is the observation space? 
   The output is Box(4,). 
   This represents a continuous space with 4 numbers. 
   Based on the problem, what could these four numbers possibly represent?
   The four numbers could possibly represent:
   1. Cart Position         - How far the cart is from the center? 
   2. Cart Velocity         - How fast the cart is moving?
   3. Pole Angle            - The tilt of the pole from vertical.
   4. Pole Angular Velocity - How fast the pole is tilting.

3. What does the reward seem to represent in this environment?
When the random agent is executed, it becomes evident that the reward amounts to 1 for each time step in which the pole stays balanced. The episode concludes when the cart strays too far from the center.The reward essentially consists of the number of steps you survive before failing.
We received two exercises to finish, with exercise 1 requiring us to set up the "CartPole-v1" environment. I copied the code from index.py and substituted the "FrozenLake-v1" environment with the "CartPole-v1" environment. In exercise 2, we needed to take the "FrozenLake-v1" script as a foundation and eliminate render(), print(), and time.remove sleep() calls from the main loop to enhance execution speed, and establish an outer loop for running 1000 episodes.Then, we needed to save the total_reward from each episode in a list. After completing the outer loop, we had to add code to compute and display the average reward for the 1000 episodes. 

Initially, while working on the exercises, it was challenging to grasp what was actually going on and how the code was executing. Over time, I practiced 2 to 3 times and repeated the exercises for submission. I came to understand it better and discovered that it was easy.
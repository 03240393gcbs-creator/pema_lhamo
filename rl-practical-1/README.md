# RL Module Practicals

##  Summary

This project includes two exercises using the Gymnasium library.

- **Exercise 1 (CartPole-v1):** Run a random agent and explore action and observation spaces.
- **Exercise 2 (FrozenLake-v1):** Run 1000 episodes with a random agent and calculate the average reward.

---

##  Exercise 1: CartPole-v1

**Action Space:** Discrete(2)  
- Two actions:  
  - 0 = Move cart left  
  - 1 = Move cart right  

**Observation Space:** Box(4,)  
It contains 4 continuous values, which likely represent:  
1. Cart position  
2. Cart velocity  
3. Pole angle  
4. Pole angular velocity  

**Reward Meaning:**  
- The agent gets +1 reward for every step the pole stays upright.  

**Total Reward in One Episode:**  
- 10


##  Exercise 2: FrozenLake-v1

**Episodes Run:** 1000  
**Average Reward:**  
- 0.015

##  Challenges Faced

- Understanding `terminated` vs `truncated` in the Gym step function.
- Making sure rendering was turned off to speed up FrozenLake testing.
- Figuring out what the 4 values in CartPole observations mean.


##  Key Takeaways

- Gym environments all use `reset()` and `step()` — very consistent.
- Random agents don’t perform well — they have no memory or learning.
- Reward is how success is measured. In CartPole, it's time balanced. In FrozenLake, it’s reaching the goal.


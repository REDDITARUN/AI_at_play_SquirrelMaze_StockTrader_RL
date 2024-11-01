# 🐿️ Squirrel Maze & 📈 Stock Trader RL Environments

Hello there! Welcome to this Reinforcement Learning (RL) project where we’re exploring two distinct environments: a **Squirrel Maze** and a **Stock Trader**. Each environment offers unique learning experiences and challenges to make our RL agents smarter. Let’s dive into the details!

Read more at: 

---

🚨Academic Integrity Disclaimer🚨
This project in this repository is intended solely as an inspiration for your future projects and should be referenced accordingly. It is not meant for students to fulfill their academic project requirements. If a student uses this project for such purposes, the creators are not responsible. The student will be solely accountable for violating academic integrity. We explicitly state that this repository should not be used to meet academic requirements. Therefore, any academic integrity issues should be addressed with the student, not the creators.

---


## 🎯 Project Highlights

- **Two RL Environments**: Deterministic and stochastic versions of the *Squirrel Maze* and a dynamic *Stock Trading* simulation.
- **RL Techniques**: We explore tabular Q-Learning, Double Q-Learning, and variations to master each environment’s quirks.
- **Customizable Parameters**: Adjust hyperparameters and see how changes affect agent performance.


## 🐿️ Squirrel Maze Environment

![image](https://github.com/user-attachments/assets/c61691a4-4085-45af-8f9b-40d04c636df9)

Imagine a squirrel navigating a 4x4 grid to gather acorns, avoid hunters, and make it home safely. Simple? Not quite! We’ve built two versions:

1. **Deterministic**: Actions are predictable; every step the squirrel takes is reliable.
2. **Stochastic**: Actions are influenced by probability (70% desired move, 10% other moves), so unpredictability keeps our RL agent on its toes!

**Environment Features**:
- **State Space**: 4x4 grid with specific states.
- **Rewards**:
  - Acorn Collection: +50 to +80
  - Goal Achievement: +10
  - Hunter Encounter: -20 to -50
  - Steps that move towards or away from the goal are rewarded or penalized.
- **Agent’s Goal**: Maximize reward by gathering acorns, reaching home, and avoiding danger.

---

## 📈 Stock Trader Environment

A perfect RL playground for those with a financial bent! Here, our agent learns to make stock trades over time, optimizing gains while navigating market highs and lows.

**Environment Features**:
- **State & Action Spaces**: Represents stock price changes over time, buy/sell/hold actions.
- **Rewards**: Based on the profit/loss of each trading session.
- **Goal**: Maximize account value by learning the dynamics of stock market trends and making smart trading decisions.

---

## 🔍 Algorithms in Action

We implemented Q-Learning and Double Q-Learning with hyperparameter tuning to refine agent performance. Here’s a peek at our approach:

- **Q-Learning**: The agent uses a single Q-table to store values for state-action pairs.
- **Double Q-Learning**: Uses two Q-tables to reduce overestimation bias, providing more reliable action evaluations.
- **Hyperparameter Tuning**: Tested max timestamps, decay rates, and learning rates to balance exploration and exploitation.

---

## 📊 Key Results

Across 1000 episodes, our agents showed:
- **Stabilized Rewards**: After training, agents consistently earned rewards aligned with their objectives.
- **Epsilon Decay**: A gradual reduction in exploration resulted in confident, policy-based actions.
- **Enhanced Learning with Double Q-Learning**: Better long-term reward stability in stochastic environments.

**Graphs and Visualizations**:
Each section includes graphs for reward trends, Q-table updates, and performance metrics so you can see how each hyperparameter adjustment influenced the agent’s learning journey!

---

## 💡 Want to Tinker?

Feel free to tweak the hyperparameters in the code to observe different learning outcomes! Here are a few starter ideas:
- **max_timestamps**: Increase for longer sessions to see how the agent adapts.
- **decay_rate**: Adjust the rate at which exploration decreases over episodes for a balanced exploration/exploitation mix.

---

## 📚 References

A huge shoutout to the resources and RL studies that guided us on this journey, including works by Hasselt, Guez, and Silver on Double Q-learning, as well as comprehensive RL comparisons between SARSA and Q-Learning.

--- 

Let’s connect! Got some cool ideas for further improvement? Or maybe you’re exploring RL yourself? Drop a line or fork this project and let’s brainstorm together. Thanks for checking it out! 😄

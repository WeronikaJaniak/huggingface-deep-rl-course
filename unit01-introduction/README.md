# Unit 1 — Introduction to Deep Reinforcement Learning

This directory contains the practical exercises and experiments completed during Unit 1 of the Hugging Face Deep Reinforcement Learning Course.

## Overview

This unit introduces the fundamental concepts of reinforcement learning and demonstrates how agents learn through interaction with an environment.

The practical assignment involves training a LunarLander agent using Proximal Policy Optimization (PPO), evaluating its performance, and publishing the trained model on the Hugging Face Hub.

## Learning Objectives

- Understand agents, environments, states, actions, and rewards.
- Distinguish between episodic and continuing tasks.
- Understand the exploration-exploitation trade-off.
- Learn the difference between value-based and policy-based methods.
- Understand the basic reinforcement learning training process.
- Train and evaluate a reinforcement learning agent.
- Publish a trained model to the Hugging Face Hub.

## Practical Exercise — LunarLander

The objective is to train an autonomous agent to control a spacecraft and land it safely on a designated landing pad.

The agent receives observations describing its position, velocity, orientation, and landing-leg contact states. It learns to select actions that maximize cumulative rewards.

### Implementation

| Component | Description |
|---|---|
| Environment | LunarLander-v2 |
| Algorithm | Proximal Policy Optimization (PPO) |
| Policy | Multi-Layer Perceptron (MlpPolicy) |
| Framework | Stable-Baselines3 |
| Environment Library | Gymnasium |
| Training Platform | Google Colab |
| Training Timesteps | 1,000,000 |

The complete PPO implementation, including model configuration,
training, evaluation, and experimental results, is available
in the accompanying Jupyter notebook.

**[View PPO LunarLander-v2 Notebook](Unit1_PPO_LunarLander_v2_Showcase.ipynb)**

### Evaluation Results

The trained agent was evaluated using the mean reward and standard deviation across evaluation episodes.

| Metric | Result |
|---|---:|
| Mean Reward | 271.67 |
| Standard Deviation | 18.98 |
| Local Evaluation Score | 252.69 |
| Official Hugging Face Score | 235.88 |
| Required Score | 200 |
| Assignment Status | Passed |

The evaluation score is calculated as:

**Score = Mean Reward − Standard Deviation**

The local evaluation achieved a score of **252.69**, exceeding the required threshold of 200.

The official Hugging Face evaluation returned a score of **235.88**, successfully validating the Unit 1 assignment.

Differences between the two scores can arise from the stochastic nature of the environment and the evaluation episodes.

## Trained Model

The trained PPO agent has been published on the Hugging Face Hub.

**Model:** [PPO LunarLander-v2](https://huggingface.co/Wjaniak2310/ppo-LunarLander-v2)

## Key Takeaways

- Implemented a deep reinforcement learning agent using PPO.
- Trained a neural network policy through interaction with a simulated environment.
- Evaluated agent performance using multiple episodes.
- Examined the relationship between average reward and performance variability.
- Published a trained reinforcement learning model.
- Successfully completed the Unit 1 practical assignment.

## References

- [Hugging Face Deep RL Course — Unit 1](https://huggingface.co/learn/deep-rl-course/en/unit1/introduction)
- [Unit 1 Practical Exercise](https://huggingface.co/learn/deep-rl-course/en/unit1/hands-on)
- [Stable-Baselines3 Documentation](https://stable-baselines3.readthedocs.io/)
- [Gymnasium Documentation](https://gymnasium.farama.org/)

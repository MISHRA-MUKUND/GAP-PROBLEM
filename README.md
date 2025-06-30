# 🧠 Deep Reinforcement Learning for the Generalized Assignment Problem (GAP)

This project applies a Deep Q-Network (DQN) to solve the Generalized Assignment Problem (GAP) using a custom OpenAI Gym environment. The objective is to optimally assign virtual machines (VMs) to servers under resource constraints while maximizing total utility.

---

## 📌 Problem Statement

The Generalized Assignment Problem (GAP) involves:
- Assigning `n` tasks (VMs) to `m` agents (servers)
- Each agent has limited capacity
- Each task has a utility and a demand per agent
- The goal is to **maximize total utility** while respecting server capacity constraints

---

## 🚀 Solution Overview

- ✅ **Custom OpenAI Gym Environment**: Models GAP with dynamic utility, demand, and capacity matrices
- ✅ **DQN Agent with LSTM**: Trained using a neural network with LSTM to handle varying server/task dimensions
- ✅ **Reinforcement Learning**: Uses Q-learning to make optimal assignment decisions based on environment state
- ✅ **Training & Evaluation**: Agent is trained on 12 datasets, each with multiple GAP instances

---

## 🧰 Tech Stack

- Python
- TensorFlow / Keras
- OpenAI Gym (Custom environment)
- NumPy, Matplotlib
- Google Colab

---

## 📁 File Structure

📦gap-drl/
┣ 📜 finalcodegap.ipynb # Main Colab notebook with training, environment, and testing
┣ 📁 datasets/ # GAP input files: utility, demand, capacities
┗ 📜 README.md # This file

## 📊 Results

- Successfully trained a DQN agent to generalize across multiple GAP datasets
- Demonstrated intelligent VM-to-server assignment strategies under constraints
- Achieved higher utility than random baseline placement

---

## ▶️ Running the Project

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/gap-drl.git
Open finalcodegap.ipynb in Google Colab

Run all cells to:

Load data

Train the DQN agent

Test on multiple GAP problem instances

📌 Future Work
Add support for PPO / A2C reinforcement learning agents
Enable real-time inference API for GAP solver



---
title: "Mario Kart Reinforcement Learning"
excerpt: "This is an AI project that teaches an agent to play Mario Kart Wii via reinforcement learning techniques. The project utilizes PyTorch and the Double Deep Q Network (Double DQN) algorithm to train a model capable of in-game decision making.<br/><img src='/images/mario_kart_ai.png'>"
permalink: /projects/mario-kart
collection: academic-projects
---

In Notre Dame's Introduction to Artificial Intelligence (CSE 30124) course, I worked on an AI project to teach an agent how to play Mario Kart Wii using reinforcement learning techniques. The project involved using PyTorch and the Double Deep Q Network (Double DQN) algorithm to create a model for in-game decision-making.

A significant part of the project used a modified version of the Dolphin Emulator, allowing Python scripting to enable interaction between the AI agent and the game. I developed a controller mechanism through Python scripting to control the racer's movements and actions.

The Dolphin Memory Engine played an important role by providing access to key game metrics such as lap progress, distance traveled, and driver speed. These metrics were used to construct the reward function for the reinforcement learning model. Integrating these metrics into the PyTorch-based model with the Double DQN algorithm helped improve the AI's learning process, focusing on achieving in-game milestones.

For further exploration, the source code is available on [GitHub](https://github.com/johnflanagan827/mario-kart-ai).

<img src='/images/mario_kart_ai_large.png'>
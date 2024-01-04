---
title: "Mario Kart Reinforcement Learning"
excerpt: "This is an AI project that teaches an agent to play Mario Kart Wii via reinforcement learning techniques. The project utilizes PyTorch and the Double Deep Q Network (Double DQN) algorithm to train a model capable of in-game decision making.<br/><img src='/images/mario_kart_ai.png'>"
permalink: /projects/mario-kart
collection: academic-projects
---


In Notre Dame's Introduction to Artificial Intelligence (CSE 30124) course, I worked on an AI project aimed at teaching an agent to play Mario Kart Wii, employing reinforcement learning techniques. This project was centered around the use of PyTorch and the Double Deep Q Network (Double DQN) algorithm to develop a model for in-game decision-making.

A key component of the project was a [fork of the Dolphin Emulator](https://github.com/Felk/dolphin), which had been modified to allow Python scripting. This modification was instrumental in enabling direct interaction between the AI agent and the game. Through Python scripting, I created a controller mechanism for the racer, facilitating its movement and actions within the game.

The [Dolphin Memory Engine](https://github.com/aldelaro5/Dolphin-memory-engine) played a pivotal role as well, as it provided access to vital game metrics such as lap progress, distance traveled, and driver speed. These metrics were essential in constructing the reward function for the reinforcement learning model. Integrating these metrics into the PyTorch-based model with the Double DQN algorithm allowed for the refinement of the AI's learning process, focusing on significant in-game achievements.

This methodological approach culminated in the AI agent successfully completing a lap with Funky Kong in the Flame Rider vehicle, showcasing the effectiveness of the learned strategies and decision-making skills.

For further exploration or to delve into the specifics of this project, the source code is available on [GitHub](https://github.com/johnflanagan827/mario-kart-ai).

<img src='/images/mario_kart_ai_large.png'>
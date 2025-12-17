# CS-370 Final Project: Intelligent Agent for Treasure Hunt Game

---
### Table of Contents
* [Jupyter Project](/Shoemaker_Joshua_ProjectTwoMilestone.ipynb)
  * [My Work Overview](#work-completed-on-the-project)
  * [My Contributions](#my-contributions-included)
* [Importance of Computer Science](#connecting-course-learning-to-computer-science)
  * [What Computer Scientists Do](#what-do-computer-scientists-do-and-why-does-it-matter)
  * [How I Approach Problems](#how-do-i-approach-a-problem-as-a-computer-scientist)
  * [Ethical Responsibilites](#what-are-my-ethical-responsibilities-to-the-end-user-and-the-organization)

  
## Project Overview
This repository contains my final project for CS-370, where I developed an intelligent agent using deep Q-learning (DQN) to navigate a pirate character through an 8x8 maze in a treasure hunt game. The agent learns to find the optimal path from the starting position (top-left) to the treasure (bottom-right) while avoiding obstacles, minimizing penalties for invalid moves, and preventing inefficient looping behaviors.

---

### Work Completed on the Project
I was provided the starte code, including:
* TreasureMaze.py: A class representing the maze environment, handling state updates, rewards, valid actions, and visualization.
* GameExperience.py: A class for storing and replaying episodes (experiences) to train the agent, implementing experience replay for stable learning.
* A [Jupyter notebook](/Shoemaker_Joshua_ProjectTwoMilestone.ipynb) with a skeleton structure, including helper functions, global variables, and a partially implemented qtrain() function.

### My Contributions included
* Completing the qtrain() function in the Jupyter notebook to implement the full deep Q-learning training loop. This involved managing exploration-exploitation via an epsilon-greedy policy, storing experiences in the replay buffer, sampling batches for training, updating the neural network model with temporal difference learning, periodically syncing a target network to stabilize Q-value estimates, and tracking metrics like win rate and loss.
* Implementing the build_model() function to create a Keras-based neural network with an input layer matching the flattened maze state, a hidden Dense layer with ReLU activation, and an output layer for Q-values corresponding to the four possible actions (left, up, right, down).
* Writing the design defense document (Shoemaker_Joshua_DesignDefense_Project2.docx) to explain the algorithm, compare human vs. machine problem-solving, justify hyperparameter choices, and discuss strengths, limitations, and ethical considerations.
* Testing and refining the model to achieve a 100% win rate after training, ensuring it passes completion checks and demonstrates efficient pathfinding.

---

## Connecting Course Learning to Computer Science

### What Do Computer Scientists Do and Why Does It Matter?
Computer scientists design, analyze, and implement algorithms and systems to solve complex problems efficiently using computation. They work on everything from developing AI models (like the DQN agent in this project) to optimizing data structures, securing networks, and advancing fields like machine learning and cybersecurity. Their work matters because it drives innovation in technology that impacts daily life—enabling smarter healthcare diagnostics, efficient transportation systems, and personalized education. In a data-driven world, computer science ensures scalable, ethical solutions to global challenges, such as climate modeling or equitable AI, fostering progress while addressing societal needs.

### How Do I Approach a Problem as a Computer Scientist?
As a computer scientist, I approach problems systematically: first, by understanding the requirements and constraints (e.g., the maze's state space and reward structure in this project); then, breaking it down into manageable components (e.g., environment modeling, agent training, and evaluation); selecting appropriate tools and algorithms (e.g., DQN for handling high-dimensional states); iterating through prototyping, testing, and refinement (e.g., tuning epsilon decay for better convergence); and validating results against metrics (e.g., win rate). This methodical, evidence-based process, informed by computational thinking, ensures robust, efficient solutions scalable to real-world applications.

### What Are My Ethical Responsibilities to the End User and the Organization?
My ethical responsibilities include ensuring transparency, fairness, and safety in systems I build. For end users, this means designing AI that avoids biases (e.g., ensuring the agent doesn't favor inefficient paths due to flawed training data) and provides clear explanations of decisions, protecting privacy and preventing harm. For organizations, I must prioritize integrity by adhering to legal standards, reporting potential risks (e.g., overfitting leading to unreliable performance), and promoting sustainable practices. In this project, ethical considerations extended to balancing AI's autonomy with user control, as over-reliance on automated agents could lead to real-world issues like financial misadvice in similar applications. Upholding these responsibilities builds trust and contributes to responsible innovation.

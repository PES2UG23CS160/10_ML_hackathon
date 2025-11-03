# 10_ML_hackathon
## 10_ML_notebook: Reinforcement Learning Agent for Hangman
Overview
10_ML_notebook demonstrates a reinforcement learning approach—specifically tabular Q-learning—to learning optimal strategies for playing the classic Hangman word-guessing game. The agent learns letter-guessing policies by interacting with a simulated environment and progressively refining its decision-making.
### Features
•	Custom Hangman environment with masked word states, tracked lives, and win/loss conditions.
•	Q-learning agent with tabular state-action value storage.
•	Epsilon-greedy exploration strategy.
•	Tunable reward functions to encourage correct letter guesses and penalize mistakes.
•	Automated training and evaluation loop with performance metrics:
o	Success Rate
o	Letter Accuracy
o	Average Wrong Guesses
o	Average Repeated Guesses
•	Plots for visualizing agent learning over episodes.
•	Modular Python code with Gradio UI for interactive testing and demo.
### Getting Started
Prerequisites
•	Python 3.7 or later
•	numpy
•	matplotlib
•	gradio
Install dependencies:
pip install numpy matplotlib gradio

### Usage
1.	Clone or download this project.
2.	Prepare your training and test corpus files (corpus.txt, test.txt)—each word on a separate line.
3.	Run the main Python script or Jupyter notebook:
python 10_ML_notebook.py

4.	Use the Gradio UI:
o	Upload your corpus file to initialize the agent.
o	Play manual games or run automated evaluation.
o	Visualize results and learning plots.
### Files
•	10_ML_notebook.ipynb — Main RL agent and environment code.
•	corpus.txt — Training corpus (word list).
•	test.txt — Evaluation word list.
•	README.md — Project documentation (this file).
•	learning_plot.png — Sample learning curve image.
### Results
After training on 1,674 words, the agent achieved:
•	Success Rate: 10.27%
•	Letter Accuracy: 58.87%
•	Avg. Wrong Guesses: 5.80
•	Avg. Repeated Guesses: 0.00
Plots of learning progression and episode rewards are included.
### Project Structure
•	HMMModel — Contextual probability estimation for letter selection.
•	HangmanEnv — Simulated episode environment.
•	QLearningAgent — RL agent implementation.
•	Gradio Blocks UI for ease of demo and testing.
### Analysis
See Analysis_Report.pdf for:
•	Key observations and challenges
•	Agent strategies and design decisions
•	Exploration/exploitation handling
•	Suggestions for future improvements


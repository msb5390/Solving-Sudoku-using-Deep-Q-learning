#  Solving-Sudoku-using-Deep-Q-learning

![](https://github.com/ADItyaP999/Solving-Sudoku-using-Deep-Q-learning/blob/master/images/DQN%20-%20Sudoku%20Solver.png)

This project is about solving Sudoku using Deep Q Learning.

The Input layer consist of 
 - Current State
 - Action being performed in Current State
 - Reward , which has been got for doing the Action
 - Future State after performing the Action

In middle I used a 2 Hidden Layers  of 20 Neurons each.

 In Output Layer the has group of actions that are needed to solve Sudoku
 - Move Action -> Those are Left,Right,Up,Down
 - Inserting Number -> Insert Numbers from 1 to 9

## Experience Memory
To Train the Neural Network the Model needs to have a proper data points. For the above problem initially I saved 200 

**[Current State , Action ,Reward ,Future State]** 

And this 200 set comes from Evaluation Network done by Program. And after 200 data points I used DQN Model i.e; Target Value and Evaluated Value for making proper predictions for further Environments.

## How to run : 
[Click Here to Downlaod the Dataset](https://www.kaggle.com/bryanpark/sudoku)

To install required packages

    pip install -r requirements.txt
Run the root.py file to start training. **Run in Terminal ONLY**

    python root.py


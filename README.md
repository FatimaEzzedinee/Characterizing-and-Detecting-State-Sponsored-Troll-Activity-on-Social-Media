# How-Troll-are-you-Measuring-and-Detecting-Troll-Behavior-in-Online-Social-Networks

Code for the implementation of the approach presented in "How Troll are you Measuring and Detecting Troll Behavior in Online Social Networks?" by Fatima Ezzeddine, Luca Luceri, Omran Ayoub, Ihab Sbeity, Ginaluca Nogara, Emilio Ferrara and Silvia Giordano

The code allows:

1. RNN-LSTM Classification.ipynb:

          - Trajectory Formation
          - LSTM Model training
          - LSTM Model evaluation
          - Troll Score Computation
          - CDF Plot for the computed scores
          
2. Troll Score Classification.ipynb:

          - Load the computed scores
          - Compute the threshold that leads to the best auc, accuracy, precision, recall, f1-score, TNR
          - Display the results

3. trajectory_main.py: Computed trajectories to the trolls (resp. users)

Initial Trajectory Extraction Code can be found here:  https://github.com/luceriluc/Detecting-Troll-Behavior-via-Inverse-Reinforcement-Learning/

Trolls-related (resp. users-related) tweets are tweets where troll (resp. user) accounts have been actively or passively involved.

The actively involved tweets are used to create the ACTIONS of the Classification includes:

          - original tweets generated by trolls (resp. users)
          - retweets generated by trolls (resp. users)
          - replies generated by trolls (resp. users)
          - mentions generated by trolls (resp. users)

The passively involved tweets are used to create the STATES of the Classification problem and includes:

          - retweets of trolls' (resp. users) generated content
          - replies to trolls' (resp. users) generated content
          - tweets where trolls (resp. users) were mentioned
          

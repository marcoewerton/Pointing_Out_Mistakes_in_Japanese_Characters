# Pointing_Out_Mistakes_in_Japanese_Characters
MATLAB code related to Section 3 (Processing Demonstrations and Assessing the Correctness of Observed Trajectories) of the paper "Assisting Movement Training and Execution with Visual and Haptic Feedback", Frontiers in neurorobotics, 2018. Link to the paper: https://www.researchgate.net/publication/324918520_Assisting_Movement_Training_and_Execution_with_Visual_and_Haptic_Feedback

To try writing a character and get visual feedback:
1) Run MainApplication.m
2) "Please Enter the name of the demonstration you want to learn!: " in the Command Window. Enter "KI" for example.
3) Write "KI" in Figure 2 using the mouse. It should look like the character in Figure 1.
4) Some plots are generated. Figure 3 shows your trial against the demonstrations. Mistakes in your trial are red. Correct points are blue. Figure 4 shows the probability density function evaluated at each position of your trial and of the mean trajectory for each stroke.
5) Press space.
6) Some other plots are generated. Figure 5 shows time step versus x and y trajectories for each stroke. Figure 6 shows time step versus score.
7) "if you want to try again type "y" or anything else otherwise: " in the Command Window. If you enter "y", you can try to write the same character again. Otherwise, you can try to write a different character.

To enter your own demonstrations:
1) Run addDemonstration.m
2) "Please enter the name of the demonstration you want to add: " in the Command Window.
3) "Please enter the amount of strokes you need to demonstrate: " in the Command Window.
4) In script_preprocess_demonstrations.m, define the variable characters_name.
5) Run script_preprocess_demonstrations.m

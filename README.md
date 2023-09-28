# rubik
Rubik's cube solver using a custom version of Thistlethwaite's algorithm 

# Approach
We're using the main principles of Thistlethwaite's algorithm detailed in this [paper](https://www.jaapsch.net/puzzles/thistle.htm).<br />
The idea is to solve certain aspects of the cube using a phase system. Those phases or cube states are defined as g0, g1, g2 and g3.<br />
The goal is to move from each phase to the next while restricting ourselves to using only a specific set of moves.<br />
In order to code this algorithms, it's possible to use lookup tables to figure out what moves to do to go to the next step. Instead we used our own methods to achieve this. For some of the steps we used hard-coded logic using "human" algorithms. For other phases, we brute forced out way to find the moves necessary to go to the next step. Brute forcing can work well here because we're not using all of the moves of the cube at once and the number of moves to go from one phase to another is not too high.<br />
Overall, the algorithm performs pretty well in terms of speed (few seconds max) and number of moves (about 52-75) needed to solve a position. 


# Credit
Made by [Florian Blanchard](https://github.com/floblanc), [Julien Dumay](https://github.com/chokmania) and myself, [Aleksi Gautier](https://github.com/kelias-42) in 2020.

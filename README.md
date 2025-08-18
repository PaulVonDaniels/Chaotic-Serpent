# Chaotic-Serpent Project: Chaotic Console Drift

The project is a visualization of the random movement of the 'O' symbol in a terminal window with a dynamic kinetic trace effect. The simulation is based on a model of Brownian motion implemented through a deterministic probabilistic change in direction (the chance of rotation is only 5% for each frame), creating the illusion of a live object behavior.

Technical specifications:
Engine: The algorithm is based on the simplest randomness generator (rand()), which shapes the behavior of an object by calculating the probability of a trajectory change using the %20 operator.
Space: Uses the toroidal geometry of an 80x30 character screen — the terminal acts as a closed world where an object moves freely without borders, leaving the screen and reappearing on the opposite side.
Trace: The movement is accompanied by a kinetic train of 42 segments forming an annular buffer, visually emphasizing the dynamics of the movement of the symbol.
Rendering: Provides a high frame rate of 60 FPS (the interval between frames is about 16(6) milliseconds).
API: The Windows API is used for implementation, providing access to low—level terminal window control and synchronization of graphic animations.

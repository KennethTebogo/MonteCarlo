# Monte Carlo Pi Estimation
This project estimates the value of Pi using the Monte Carlo method, with a graphical visualization using the vpython library. The program simulates throwing random points (representing "stones") inside a square and calculates the proportion of points that land inside a quarter circle to estimate Pi.

# Project Overview
The program generates random coordinates within a square.
It checks if the generated point falls inside a quarter circle inscribed within the square.
The ratio of points inside the circle to the total points is used to estimate Pi.
The process is repeated for multiple iterations to average the Pi estimate and visualize the simulation in real-time.

# Features
Monte Carlo simulation to estimate Pi.
Real-time graphical visualization of the points thrown inside the square.
The points inside the circle are displayed in red, and the points outside the circle are displayed in blue.
The Pi estimate is updated continuously on the graph as more points are thrown.

# Requirements
Python 3.x
vpython library for 3D and graphical visualizations
random and math libraries (standard Python libraries)
Install the required packages:

bash
```
pip install vpython
```
How to Run the Program
Clone the repository to your local machine (or simply create a Python file with the code).

Make sure you have the necessary libraries installed (vpython).

# Run the Python script:

bash
```
python3 MonteCarlo.py
```
Watch the simulation run, throwing points and calculating Pi.
Code Explanation
# Inputs:

x_coord, y_coord: Coordinates of the thrown stone.
maxit: Number of "stones" (random points) thrown in each simulation.
rad: Radius of the quarter circle (usually 1).
square: The area of the square in which points are thrown (usually 2).
M: Number of times the simulation runs (for averaging Pi).

# Processing:

The program simulates throwing maxit random points inside the square and checks whether each point falls within the quarter circle.
The ratio of points inside the circle to total points is used to estimate Pi, calculated as Pi ≈ 4 * (inside points / total points).
This process is repeated M times, and the average Pi value is computed.

# Graphical Visualization:

gdisplay and gdots from the vpython library are used to visualize the points on a 2D graph.
Points inside the circle are plotted in red, and those outside the circle are plotted in blue.
The current estimate of Pi is plotted on a separate graph in real-time.

# Output:

After all iterations, the program prints the estimated value of Pi and the absolute error between the estimated Pi and the actual Pi.
Example Output
bash
```
Pi estimate = 3.1416
Absolute error = 0.000130899
```

# Contributions
Feel free to fork the repository and submit pull requests if you have any improvements or bug fixes.

# License
This project is licensed under the MIT License.

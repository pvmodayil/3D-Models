# 3D-Models
.f3d models of various objects for various projects
$(\tilde{x}_i, \tilde{y}_i)$

# Coding Exercise: Aerodynamic Uncertainties of Reusable Launch Vehicles (Vacancy 78414)

## Instructions

This short coding exercise shall mimic some common tasks that may occur during the internship. 
The purpose of this exercise is actually _not_ to challenge you with some very complex tasks, but rather to get some general feeling about your experience with Python and Software Engineering.
Therefore, solutions which are simple, user-friendly, maintainable and _pythonic_ - which follow your understanding of _best practices_ - are generally preferred over complex, mind-blowing or unconventional pieces of code.

You can find the individual tasks of this exercise in the section below.
Please note that the formulation of some tasks is purposely quite open, to give you some room for interpretation and the freedom to decide.
If you are in doubt what is actually requested, just go with the most practicable approach.
Don't assume there is _one right_ solution.

Please store all your results in the git repository, that you will create in exercise 1).
We would like to ask you to mail us this repository, containing all your solutions, until **Monday, 27. March 2023, 14:00 CET** latest.
To create a transferable version of your repository, please use the [`git bundle create repo.bundle --all`](https://stackoverflow.com/a/11795549) command and simply attach the `*.bundle` file to your mail.

**Please do not push your repository to a public server (e.g. GitHub), so we can ensure equal conditions for all candidates.**

Feel free to use any tools that you like and that you are comfortable with for solving this exercise. We would only like to request you:
* To prepare all solutions **yourself**;
* To not spend more than **max 2h** on these tasks; (we know, there are always things to improve - but please be advised that you won't gain any advantage if you waste your weekend)
* To use **Python** for all source code.

Besides that, we are very excited to receive your solutions soon - Good luck and happy coding! :)

## Exercise

Your colleague Daisy has set up a new, cutting-edge, but resource-intensive data generation process.
This process is approximating a complex functional relation $y=f(x)$, but every time she draws samples $(\tilde{x}_i, \tilde{y}_i)$ from the process, some random errors are added to the data.

You actually don't fully understand her process yet, but as an excellent data scientist you know some simple tricks to deal with noisy data.
Therefore, Daisy agreed to share with you some fresh samples every other week, if you implement some helpful Python functions that both of you can use.

### 1) Setup git repository

Create and setup a new git repository for developing your Python code.
You may add some structure to the repository to better organize its content.
Please use this repository for storing your code for all subsequent tasks, assuming that you and Daisy may want to work on it in parallel.

### 2) Implement function: Mean & confidence interval

Implement a function which takes an arbitrary table of data samples $(\tilde{x}_i, \tilde{y}_i)$ from Daisy's process and returns the mean, as well as the upper and lower boundary of the confidence interval, for each given $\tilde{x}_i$.
The confidence level shall default to 75%, but may optionally be set by the user.

### 3) Implement function: Simple regression model

Implement a _simple_ regression model for Daisy's data.
For better usability, cast this model in a function which takes a table of training data (as in 2) ) and some new values $\hat{x}_j$ as input, and returns the corresponding prediction values $\hat{y}_j$.

_Note: It is not necessary to implement a complex or detailed model here; It is more about the approach that you would follow._

### 4) Implement function: Plotting

Implement a function that returns a plot of Daisy's data, given the table of data samples (as in 2) ) for input.
If optionally also mean and confidence interval data (from 2) ) or prediction data (from 3) ) will be provided to the function, it overlays curves for these data on the plot.

### 5) Demonstrate & Document

Demonstrate the usability of the functions implemented in 2) - 4) based on the given `sample.csv` dataset.
Please note that each column $y_i$ corresponds to a new sample from Daisy's process.
Also, describe _briefly_:
* How to use your functions;
* How to reproduce your demonstration case;
* Which tools you have used for development;
* What would you improve next, if you had more time.

_Note: KISS - Keep it simple stupid_

---
Copyright (c) 2023 Deutsches Zentrum fuer Luft- und Raumfahrt e.V. (DLR), Germany.

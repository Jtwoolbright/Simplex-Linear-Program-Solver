# Simplex Linear Program Solver

## Background

A Linear Program is a method of maximizing or minimizing an equation based off a set of constraints that is often used to express optimization problems in the field of Operations Research (See https://en.wikipedia.org/wiki/Linear_programming to learn more). 
As more and more constraints and variables are introduced, Linear Programs can grow substantially in size, and it can be very difficult, if not impossible, to solve these problems by simple methods such as elimination or substitution. Fortunately, a US Army Air Force veteran and mathematical scientist by the name of George Dantzig discovered an easier way of solving these problems which he named the Simplex Algorithm (See https://en.wikipedia.org/wiki/Simplex_algorithm). The Simplex Algorithm is effective at solving a large subset of Linear Programs and has since been built upon to solve many more.

## Description

![StandardForm](https://user-images.githubusercontent.com/48270610/107437223-810a7a00-6ae3-11eb-916d-d866eddcf121.PNG)

The Simplex Linear Program Solver uses the original Simplex Algorithm, and it requires the Linear Program to be in standard form prior to user input (See above image). The q<sub>n</sub> is referred to as the right hand side constraints when prompting for user input, and it cannot include numbers that are <= 0. The p<sub>k</sub> is referred to as the the constants of the equation to maximize, and they also cannot be <= 0. The a<sub>nk</sub> is referred to as the constraint variable constants, and the user must type in constants for all variables, including those with zero constants, in the constraints.
  
## Requirements

![CommandLine](https://user-images.githubusercontent.com/48270610/107435750-6b945080-6ae1-11eb-86a3-b4379599acea.PNG)

To run from command line, you must have a Java kit installed and your system's environment variables properly configured. You can also run it by uploading the files to an online java environment such as https://www.onlinegdb.com/online_java_compiler.

## Output

![Output](https://user-images.githubusercontent.com/48270610/107436007-caf26080-6ae1-11eb-8de9-0b52bca7abfe.PNG)

The above output is the result from a standard LP,

Maximize P = 3x<sub>1</sub> + 5x<sub>2</sub>

Subject to: 

  x<sub>1</sub> <= 4

  2x<sub>1</sub> + 3x<sub>2</sub> <= 12
           
  2x<sub>2</sub> <= 18
  
And: x<sub>1</sub>, x<sub>2</sub> >= 0

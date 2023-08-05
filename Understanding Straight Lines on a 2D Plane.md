# Understanding Straight Lines on a 2D Plane: Slope-Intercept and General Form Equations

## Abstract

This paper aims to provide a comprehensive understanding of straight lines in a two-dimensional Euclidean space. Specifically, it explores the slope-intercept form (`y = mx + b`) and the general form (`ax + by + c = 0`) equations used to represent straight lines on a 2D plane.

In the slope-intercept form, `y` represents the dependent variable, while `x` represents the independent variable used for prediction. The coefficient `m` denotes the slope, which represents the rate of change in the dependent variable with respect to changes in the independent variable. The coefficient `b` indicates the y-intercept, representing the value of the dependent variable when the independent variable is 0.

The general form equation, `ax + by + c = 0`, employs coefficients `a`, `b`, and `c`, determining the position and direction of the straight line in the 2D plane. Coefficients `a` and `b` are equivalent to the slope in the slope-intercept form, while `c` is a constant affecting the position of the line.

The paper also discusses the transformations between the slope-intercept and general form equations. Specifically, the slope-intercept form can be transformed into the general form, and vice versa.

Furthermore, the glossary section provides key terms related to straight lines in 2D, including explanations of the dependent and independent variables, slope, y-intercept, and the distinction between vertical and horizontal lines. Additionally, the definitions of valid lines and how to represent them in different forms are covered.

Overall, this paper serves as a valuable resource for comprehending the fundamental concepts and representations of straight lines on a 2D plane, providing essential knowledge for various fields, including mathematics, physics, and engineering.



On a flat plane which is also known as a two dimensional Euclidian space, the slope-intercept of a straight line can be defined by the equation `y=mx+b`.

- `y`: This is the variable or value that we are trying to predict or estimate. It is also called a dependent variable.
- `x`: Is the value or a variable which is being used for the prediction. It's also called the independent variable.
- `m`: Is the representation of the change in `y` for changes in each unit of `x`. In essence it represents the rate of change in the dependent variable compared to the independent variable. This is called the slope.
- `b`: Is the value of the dependent variable when the independent variable is 0. Visualize this as the point where the line crosses the y-axis. This is called the y-intercept.

The changes in `m` and `b` changes the slope and position of the line in the Ecuclidian space. 

The above equation can be transformed into a general form represented as `ax + by + c = 0`. 

- `x, y`: Are the coordiantes in two dimensional Euclidian space corresponding to the horizontal and vertical axis
- `a, b, c`: Determine the position and direction/orientation of the line. They are also called coefficients
    - `a, b`: Are the slope
    - `c`: Is the y-intercept and is a constant
    
The equation can be re-arrannged as `y = -(ax + c) / b` if `b` does not equal to 0. If the coeffcients `a` and `b` are 0 then it is not a valid line in the xy-plane. If `b` is 0 and `a` is not 0, a vertical line is represented. Inversely, if `b` is  not 0 and `a` is 0 then a horizontal line is represented. 

## Glossary
Key terms related to straight lines in 2D:

- `y`: The dependent variable or value to be predicted in the equation `y = mx + b`.
- `x`: The independent variable used for prediction in the equation `y = mx + b`.
- `m` (slope): Represents the rate of change in the dependent variable `y` for each unit change in the independent variable `x`.
- `b` (y-intercept): The value of the dependent variable `y` when the independent variable `x` is 0. It is the point where the line crosses the y-axis.
- General Form: The equation of a straight line represented as `ax + by + c = 0`, where `a`, `b`, and `c` are coefficients that determine the position and direction of the line in the 2D plane.
- `a` and `b`: Coefficients representing the slope of the line. If `b` is not 0, the equation `y = -(ax + c) / b` can be used to express the line in slope-intercept form.
- `c`: A constant in the general form equation that affects the position of the line.
- Vertical Line: A line represented by an equation where `b` is 0 and `a` is not 0. It is parallel to the y-axis and has an undefined slope.
- Horizontal Line: A line represented by an equation where `a` is 0 and `b` is not 0. It is parallel to the x-axis and has a slope of 0.
- Valid Line: A line with non-zero coefficients `a` and `b` in the general form equation. A valid line represents a unique slope and position in the 2D plane.


```python
import matplotlib.pyplot as plt
import numpy as np

# Ask the user for the slope and y-intercept
m = float(input("Enter the slope (m): "))
b = float(input("Enter the y-intercept (b): "))

# Generate an array of x values
x = np.linspace(-10, 10, 400)

# Calculate the corresponding y values
y = m*x + b

# Create the plot
plt.figure(figsize=(8, 6))  
plt.plot(x, y, label=f'y={m}x+{b}')

# Add a title
plt.title('Line graph for y=mx+b')

# Add X and y label
plt.xlabel('x')
plt.ylabel('y')

# Show legend
plt.legend()

# Show the plot
plt.show()

```

    Enter the slope (m): 3
    Enter the y-intercept (b): 2
    


    
![png](output_2_1.png)
    



```python

```

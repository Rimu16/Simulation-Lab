## Personal Information
*Name:* Farhana Yeasmin Rimu  
*ID:* 2215151009  
*University:* UITS (University of Information Technology and Sciences)  
*Department:* Computer Science and Engineering (CSE)  
*Batch:* 51  
*Section:* 7A1   

## Course Details
*Course Code:* CSE 413  
*Course Name:* Simulation and Modeling Lab  
*Course Teacher:* Audity Ghosh, Lecturer, Department of Computer Science and Engineering, University of Information Technology and Sciences (UITS)

## Assignment - 01
## Tasks
01. Generate two vectors with 15 random floats, plot them, and label axes.
02. Create a 4x4 random matrix, visualize as a heatmap, and label rows/columns.
03. Generate two 4x4 matrices, perform arithmetic operations, visualize with bar plots.

## Explanation of the Codes:
For Question 01:
01. np.random.rand(15) creates 15 random floating numbers between 0 and 1 for each vector.
02. np.arange(len(vector1)) generates an index array [0, 1, 2, ... 14] for the x-axis.
03. plt.plot() is used to plot the vectors with markers and linestyles for better visualization.
04. plt.xlabel(), plt.ylabel(), and plt.title() add axis labels and a title.
05. plt.legend() adds a legend to distinguish between the two vectors.
06. plt.grid(True) adds a grid for better readability.
07. plt.show() displays the graph.

For Question 02:
01. np.random.rand(4, 4) creates a 4x4 matrix with random numbers.
02. row_labels and col_labels are used to label the rows and columns.
03. sns.heatmap() creates the heatmap, annot=True: Shows values in each cell, cmap='coolwarm': Applies a color scheme, linewidths=0.5: Adds grid lines, xticklabels and yticklabels: Assign custom labels.
04. plt.title() adds a title, and plt.show() displays the heatmap.

For Question 03:
01. Two 4x4 matrices (A and B) are created using np.random.randint(0,25) with values between 0 and 25.
02. Each matrix is flattened into a 1D array using .flatten() for visualization.
03. Results of the operations are plotted in a 1x3 grid of subplots using plt.subplots().
04.plt.tight_layout() adjusts spacing between subplots.

Discussion of Effects:

Addition :
Combines corresponding elements of A and B. 

Subtraction :
Represents the difference between corresponding elements of A and B. It shows how much A deviates from B.

Multiplication :
Represents the dot product of A and B. It reflects the combined linear transformation of the two matrices.

## Concepts Covered
- Random number generation
- Data visualization with Matplotlib
- Matrix operations with NumPy
- Heatmap visualization
- Bar plot representation of matrix computations

## What I Learned
- How to generate and manipulate random numerical data in Python.
- Effective use of Matplotlib for visualizing mathematical operations.
- Understanding of matrix operations and their effects.
- How to present data using heatmaps and bar plots.
- Best practices for structuring a professional GitHub repository.



## Assignment - 02
## Tasks
01. Use numpy to create a 3×3 matrix of random integers between 1 and 50.
02. With a fixed seed (`np.random.seed(10)`) to ensure reproducibility.
03. Without setting a seed, allowing random values to change each time.

## Explanation of the Codes:
For Question 01:
01. This imports the NumPy library, which is used for numerical computing.
02. np.random.randint(1, 50, (3, 3)) generates a 3×3 matrix with random integers.
03. 1 is the inclusive lower bound.
04. 50 is the exclusive upper bound.
05. (3, 3) specifies the matrix size.
06. Displays the generated 3×3 matrix on the screen.

For Question 02:
01. np.random.seed(10) - random seed to 10, ensuring that the same random numbers are generated each time the code is run.
02. Since the seed is fixed, this matrix will always be the same every time you run the code.

For Question 03:
01. np.random.seed(None) - This ensures that the random number generator uses a new random starting point every time the code runs.
02. Since no fixed seed is set, the numbers will change every time you run the code.

## Difference Between The Two Output
01. Reproducibility:
Seeded: Output is reproducible and consistent across runs.
Non-Seeded: Output is not reproducible and changes every time.
02. Randomness:
Seeded: The sequence of random numbers is deterministic.
Non-Seeded: The sequence of random numbers is truly random.
03. Use Cases:
Seeded: Used when consistent results are needed.
Non-Seeded: Used when variability is required.

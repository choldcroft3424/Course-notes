Matlab = Matrix laboratory

`clc` - Clear command window (does not clear anything else from memory)
`clearvars` - Clears all variables from memory
`clear` followed by variable name will just clear that variable.
`close(figure)` will close a figure (A figure meaning a plot/graph)
`close all` will close all figures

`min(x)` returns the minimum value in the array `x`
`max(x)` returns the maximum value in the array `x`

`~` acts similarly to `_` convention in C parameters, it is used in function arguments to indicate a placeholder.

`who`- Display variable names
`whos`- Display variable names and sizes
You can double click on a variable in the workspace to view it as a spreadsheet (useful for matrices)

End line with `;` to suppress output (no output will occur).

Run a matlab script using `Ctrl+Enter`.

Comment using % `%This is a comment`

### Arrays
Define an array manually the same way you would in C. You can omit commas if you want:
![[Pasted image 20261004211505.png]]

Define an array from x to y with `x:y`
Example:
![[Pasted image 20261004210549.png]]

You can insert another number in the middle to describe the increment between each element:
![[Pasted image 20261004213047.png]]
In the above example, matrix `x` starts at 5, goes up by 3 each time, and finishes when it reaches 17.

Transpose a matrix `x` with `x'`. (Apostrophe after x. Swap rows and columns)

Use `linspace(start, end, number)` to generate an array of `number` evenly spaced numbers between `start` and `end` inclusive (if no `number` is given, the default is 100).
Example:
![[Pasted image 20261004211135.png]]
*Remember linspace means linear spacing*

Define matrices the same way you define arrays. Use a semicolon `;` to create a new row:
![[Pasted image 20261004211639.png]]


Matlab follows the rules of linear algebra, e.g. you can multiply matrices by a scalar value...
![[Pasted image 20261004211911.png]]

... But can't multiply matrices with incompatible dimensions.

![[Pasted image 20261004212022.png]]

Put a full stop `.` before the operation to apply that operation to each element in the matrix (instead of the matrix itself):
![[Pasted image 20261004212338.png]]

You can use shorthand functions `zeros(rows, cols)` and `ones(rows, cols)` to create matrices of size (`rows`, `cols`) filled with zeroes and ones respectively:
![[Pasted image 20261004212655.png]]

Use `eye(size)` to create an identity matrix of dimensions (`size`, `size`).
![[Pasted image 20261004212846.png]]


Pick an element from a matrix called `M` by using the syntax `M(rows, cols)`:
![[Pasted image 20261004213535.png]]
**NOTE:: Indexes start at 1, NOT 0**.

You can grab the last element of a matrix `M` using `M(end)`
![[Pasted image 20261004213752.png]]

You can also do `end - x` to move backwards `x` spots:
![[Pasted image 20261004214059.png]]
(In the above example, the `end` is element 9. We go back (upwards, since rows are made before columns) first to 6, then to 3. `end-3` would loop back to the next column and give you 8.)

Picking values from matrices gives a reference, so setting the value will set it in the matrix:
![[Pasted image 20261004214326.png]]

Extract an entire row or column by using `:` (the `:` signals that you want everything in that row or column).
![[Pasted image 20261004214528.png]]

You can also use the colon in this context like explained above.

Use `plot(x,y)` to plot array `x` against array `y`. It is good practice to call `figure` before `plot` since this creates a new plot instead of erasing the previous one.

Find matlab functions and get help on the [matlab documentation](https://uk.mathworks.com/help/index.html?s_tid=CRUX_lftnav).

Define anonymous functions (basically function pointers to a lambda expression) using the syntax `y = @(x) (expression)` Where y is the function pointer, x are your parameters and the expression is something like `x.^2`.

Use `xlim([min, max])` and `ylim([min, max])` to set the bounds of the x and y axes.

Use `fplot(function, xlim)` to plot a function instead of `plot` as this can handle undefined values and give a more accurate representation of what your function looks like.
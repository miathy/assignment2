# assignment2
ASK
back to top
In this assignment, your task is to create a simple line chart program using Python turtle graphics. The data for line chart will come from user input – it will be a sequence of integers in the range [0, 20].

At the program start, you should set turtle animations to be fastest, and make the turtle hidden. Next your program should implement the following requirements.

Prompt the user for the total number of points in the sequence.
Draw the layout of the chart, including the xy axis, the axis tick marks and tick labels (refer to the demo video below). Note that the number of tick marks on x-axis is not fixed, it is equal to number of data points. Y-axis, on the other hand will always have six ticks, labelled 0, 4, ... 20.
Prompt the user for individual data values, one after the other.
For each data point, draw a square marker on the chart, and a line connecting to preceding data point (if any).
To clearly understand the program requirements, watch this demo video. You should aim for similar styles and colours.

Constraints

In your program, you can only import the turtle library module.

In many online examples of turtle graphics applications, multiple turtle objects are used on the same window. You are NOT allowed to proceed that way. Use a single turtle for all drawings.

You should follow good programming practices, for example using named constants, creating several reusable functions (top-down design) and minimizing the use of global variables.

Suggested dimensions

Window size: 500 × 500
Length of Axis: 400
Origin point: (–200, –200)

Sample Codes

All the turtle functions can be called after importing the turtle module.

(1) To change the window size

turtle.setup(window_width, window_height)
(2) To write text

# can replace 'normal' with 'bold' or 'italic'. Similarly, can adjust the align argument
turtle.write('hello world', align='center', font=('Arial', 20, 'normal'))
(3) To get a number input via dialog box

value = turtle.numinput('dialog title', 'message', minval=0, maxval=20)
(4) To draw a square marker

turtle.shape('square') # do it once
turtle.stamp() # stamp the turtle at its current location
(5) OPTIONAL - To disable turtle animations (instantaneous drawing)

turtle.tracer(5)
Above statement will cause all turtle drawings to be done in batches of 5 steps. Sometimes it may cause a problem that a drawing does not show up on screen when you expect. In those cases, call turtle.update() to force draw all pending steps.

---

Your assignment should consist of the following tasks.


# WhiteboardusingJS

I first initialize the canvas element, the buttons, and the drawing context. Then, I create two variables, **drawing** and **objects**, to keep track of the current drawing state and the list of drawn objects.

Next, I attach event listeners to the canvas element and the buttons. These event listeners will call the corresponding functions when the user interacts with the whiteboard.

I then define the startDrawing(), draw(), stopDrawing(), clearWhiteboard(), handleUndo(), redrawCanvas(), and addObjectToCanvas() functions.

The startDrawing() function is called when the user clicks on the canvas. I set the drawing variable to true and initialize the tempPath variable to an array containing a single point, the point where the user clicked.

The **draw()** function is called when the user moves the mouse while the mouse button is pressed. I add the current mouse position to the tempPath array.

The **stopDrawing()** function is called when the user releases the mouse button. I add the tempPath array to the objects list if the array has more than one point. I then clear the tempPath array.

The **clearWhiteboard()** function clears the objects list, which effectively erases the whiteboard.

The **handleUndo()** function removes the last object from the objects list and redraws the canvas.

The **redrawCanvas()** function clears the canvas and then redraws all of the objects in the objects list.

The **addObjectToCanvas()** function adds a new object to the objects list. An object is simply an array of points.

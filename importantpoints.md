
->If you see the code for the rope.js .
    ● In the constructor() we are taking two parameters
    nlinks - number of links and pointA - points of connection.

    in this constructor we are creating multiple rect for having the look of rope

    we are giving points where it needs to be attached
    -------------------------------
    Using Composites.stack() function we create the multiple
rectangular bodies and store it in the rect variable.
------------------------------------
Using the Composites.chain() function we create the
chain of the rectangles.

-------------------------------------------------
n using the Constraints.create() we add the
constraints to the chain which connects all the bodies of
the chain together like we have string in a necklace.
-------------------------------------------------
IN sketch.js
While creating the object first we write the length of the
rope which we will set as 7, and then the x and y position,
x would be 245 and y as 30.
rope = new Rope(7,{x:245,y:30});

The next step is to call the rope.show() function in the
draw() function so that we can see the rope hanging.

--------------------------------------------------
we first create fruit_options for
the fruit body. In the options, we are only defining the
density of the fruit as 0.001.

we create a fruit body using the Bodies.circle()
function,we need to provide the x and y positions
and the radius of the fruit along with fruit_options.
-----------------------------------------------
in rope.js
e break() function which helps us to break the
chain.It simply makes the rope body null.
For our code we are only going to use the rope.js to
create the rope and break() function to break the rope
when the user clicks on the cut button(which will be added
in upcoming classes).

-------------------------------------------------





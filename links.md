https://brm.io/matter-js/docs/

https://brm.io/matter-js/docs/classes/Composite.html

https://p5js.org/reference/#/p5/beginShape

https://p5js.org/reference/#/p5/vertex



The Matter.Render
------------------
 module is a simple HTML5 canvas based renderer for visualising instances of Matter.Engine. It is intended for development and debugging purposes, but may also be suitable for simple games. It includes a number of drawing options including wireframe, vector with support for sprites and viewports

Typically, wireframes are static design artifacts created for a specific viewport (desktop, tablet, or mobile)
it is use for responsive design
you developed app is responsive for all size of screen


Matter.Constraint
-----------------
The Matter.Constraint module contains methods for creating and manipulating constraints. Constraints are used for specifying that a fixed distance must be maintained between two bodies (or a body and a fixed world-space position). The stiffness of constraints can be modified to create springs or elastic.

Matter.Constraint.create(options) → Constraint
Creates a new constraint. All properties have default values, and many are pre-calculated automatically based on other properties. To simulate a revolute constraint (or pin joint) set length: 0 and a high stiffness value (e.g. 0.7 or above). If the constraint is unstable, try lowering the stiffness value

constraint.bodyABody
The first possible Body that this constraint is attached to.
Default: null

constraint.bodyBBody
The second possible Body that this constraint is attached to.
Default: null


Matter.Composite
-----------------
They are a container that can represent complex objects made of multiple parts, even if they are not physically connected. A composite could contain anything from a single body all the way up to a whole world.



Matter.Composite.create([options]) → Composite
Creates a new composite. The options parameter is an object that specifies any properties you wish to override the defaults.


Matter.Composite.add(composite, object) → Composite

Parameters
composite Composite
object Object | Array

Generic single or multi-add function. Adds a single or an array of body(s), constraint(s) or composite(s) to the given composite

Matter.Composites
------------------
The Matter.Composites module contains factory methods for creating composite bodies with commonly used configurations (such as stacks and chains).

Matter.Composites.stack(xx, yy, columns, rows, columnGap, rowGap, callback) → Composite
Create a new composite containing bodies created in the callback in a grid arrangement. This function uses the body's bounds to prevent overlaps.
Parameters
xx Number
yy Number
columns Number
rows Number
columnGap Number
rowGap Number
callback Function
Returns
Composite A new composite containing objects created in the callback



Matter.Composites.chain(composite, xOffsetA, yOffsetA, xOffsetB, yOffsetB, options) → Composite
Chains all bodies in the given composite together using constraints.

Parameters
composite Composite
xOffsetA Number
yOffsetA Number
xOffsetB Number
yOffsetB Number
options Object
Returns
Composite A new composite containing objects chained together with constraints











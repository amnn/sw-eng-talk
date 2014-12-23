# Exercises

## Drawing a Triangle
Firstly, let us try and draw an equilateral triangle, in Scratch.
Remember:

 * All the sides must have the same length
 * All the angles must be the same

For this, we want to use the tools in the *Pens* and *Motion* sections.

### New Commands
#### Pen
 * `clear` Removes all pen marks from the screen.
 * `pen down` Place the pen down, so that movement causes a pen mark to
   appear in the path the sprite moves along.

#### Motion
 * `move` Move the sprite a set number of steps.
 * `turn (right)` Turn the sprite by a set number of degrees right.

### Hints

 * Don't forget to use the `When (Flag) clicked` event to start your animation.
 * You may find it useful to reset the screen before you draw the triangle.
    - `go to x: 0 y: 0` (from _Motion_)
    - `point in direction 90` (from _Motion_)
    - `clear` (from _Pen_)
 * Think carefully about the angle to turn by, the most obvious one may not
   work, so perhaps try sketching it out on paper. Maybe the angle you want
   is related to it in some way?

## Drawing a Square
Modify your code for drawing a triangle so that it draws a square instead.

 * Do you notice that you had to change multiple commands in the same way?
 * What about the pattern in the commands, is there a set of commands that
   is repeated again and again?
 * How is the angle we turn by related to the number of sides in the shape?

## The `repeat` command

We can simplify our code using the `repeat` command. `repeat` takes a number,
and a sequence of commands, and it runs the sequence repeatedly, that number
of times.

Use the answers to the questions from the previous section to convert your
square drawing code so that it uses a `repeat` block.

## Variables

Introduce a `sides` variable (see the `Data` section). Before the repeat
command, we will set it to the number of sides we are going to draw.

Replace numbers in the rest of the code with mathematical operations involving
the `sides` variable, where you think they make sense.

## Spirals

![Spirals](https://raw.githubusercontent.com/asQuirreL/sw-eng-talk/master/Spirals.png)
Instead of just drawing shapes, let us instead draw some spirals (see picture).

Spirals look very similar to the shapes we were drawing before, the only
difference is that every time we draw a side of the spiral, it is slightly
larger than the one before it.

We can do this by introducing another variable, representing the length of the
side, and adding to it at the end of every go round of the `repeat`.

Can you figure out which commands need to be modified to include this new
variable?

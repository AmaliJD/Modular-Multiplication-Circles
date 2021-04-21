# Modular-Multiplication-Circles

Use this link (https://amalijd.github.io/Modular-Multiplication-Circles/) to try the program out or download an executable.
If you have Unity, you can download these files and mess around in the code.

How to use
Slider1:
This determines how many segments the circle is cut into. The value is an integer and can range from 2 to 1000.

Slider2:
This determines which number's multiples to draw lines out of. This number can be from 0 to the number of segments.

Snap:
Snap slider 2 to integer values.

%:
Set slider 2 to a percentage of number of segments.

Animate:
Increase slider 2 over time. Use the slider to change the speed.

Dropdown Menu:
Change color mode.

Width:
Width of lines

ColorModes:
Cycle - color cycles through all hues
Length - color of line based on length of line
Position - color of line based on position on circle
Angle - color of line based on angle from positive x-axis
Gray - grayscale color

Shape:
This one is probably the most difficult to understand. There are specific 'shapes' that can be made at certain configurations. For example, setting slider2 to (slider1 / 2)-1 will give you a rectangle formation.

When you change slider1, this formation will be lost. With shape toggled on, when changing slider1, the program will find the slider2 value corresponding to the same shape.

You won't always be able to tell what the shape slider value should be and sometimes, the value may be higher than the slider's limit, but I've observed some patterns to help you. You should set the color mode to 'length' to see these patterns more easily. So, in this color mode, you can sometimes see concentrations on magenta along the perimeter of circle. The number of these concentrations should correspond to the shape slider number. Another shape is the circle. For circles, you can count the number of rings, and the shape slider value will be # rings * 2 (+1 if this formation doesn't have rays coming out the center).

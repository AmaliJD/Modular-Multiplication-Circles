# Modular-Multiplication-Circles

Use this link (https://amalijd.github.io/Modular-Multiplication-Circles/) to try the program out or download an executable.
If you have Unity, you can download these files and mess around in the code.

# How to use
### Slider1:
This determines how many segments the circle is cut into. The value is an integer and can range from 2 to 1000.

### Slider2:
This determines which number's multiples to draw lines out of. This number can be from 0 to the number of segments.

### Snap:
Snap slider 2 to integer values.

### %:
Set slider 2 to a percentage of number of segments.

### Animate:
Increase slider 2 over time. Use the slider to change the speed.

### Dropdown Menu:
Change color mode.

### Width:
Width of lines

### ColorModes:
Cycle - color cycles through all hues

Length - color of line based on length of line

Position - color of line based on position on circle

Angle - color of line based on angle from positive x-axis

Gray - grayscale color

### Shape:
This one is probably the most difficult to understand. There are specific 'shapes' that can be made at certain configurations. For example, setting slider2 to (slider1 / 2)-1 will give you a rectangle formation.

When you change slider1, this formation will be lost. With shape toggled on, when changing slider1, the program will find the slider2 value corresponding to the same shape.

You won't always be able to tell what the shape slider value should be and sometimes, the value may be higher than the slider's limit, but I've observed some patterns to help you. You should set the color mode to 'length' to see these patterns more easily. So, in this color mode, you can sometimes see concentrations of magenta along the perimeter of circle. The number (or the number+1) of these concentrations should correspond to the shape slider number. Another shape is the circle. For circles, you can count the number of rings, and the shape slider value will be # rings * 2 (+1 if this formation doesn't have rays coming out the center).

Here's how the shape slider actually works. The shapes that are produced are caused by slider2 being an CONSTANT VALUE away from producing a rational fraction with slider1. For example, setting S1 = 50 and S2 = 24 gives a rectagle shape formation. This is because 24 is 1 less than 25 which is exactly half of 50. So, for the same shape at S1 = 100, S2 should be 49. With a shape slider value of 2, the program knows the desired shape is caused by S2 being a constant value away from either (1/2) of S1 or (2/2) of S1. In this case, S2 is 1 less than 1/2 of S1. If the shape slider value was 3, the program would try to find the closest 3rd (1/3, 2/3, or 3/3) that S2 is to S1, and then save the constant value from that ratio. So again with S1 = 50 and S2 = 24, but with the shape value at 3. 24 is 7.33 more than 1/3 of 50. When we slide S1 to 100, S2 will be 40.67 since 40.67 is 7.33 more than 1/3 of 100. Unfortunatly, this relationship isn't what causes the rectangle shape formation, and you will lose the rectangle shape. This relationship does however preverse a different, but less apparent, shape. The shape slider will always preserve some underlying shape, but if you want to preserve a specific shape, you need to know the shape value to use. Typically, the most promonent shape is governed by it's relationship to the closest ratio. So if you see a very pleasing shape and the S2/S1 ratio is closest to 3/5, the shape value should be 5. So as a final example, we can look at the shape when S1 = 100 and S2 = 61. 61 is closest to 3/5 of 100. So the shape value should be 5. Sliding the S1 value, the circle shape is preserved. The specific relationship is S2 is 1 more than 3/5 of S1. If you had the shape value to 7, the program would set S2 = 3.857 more than 4/7 of S1, which doesn't preserve the circle shape.

Fun fact, my favorite shapes, the circles, are all produced by S2 being exactly 1 more than a clean fraction of S1. So 1 more than 1/4 of S1 or 1 more than 5/8 of S1, they're all circles!

I hope I explained that well enough and that you could understand it :P

## Screenshots
![alt text](https://github.com/AmaliJD/Modular-Multiplication-Circles/blob/main/Images/Screenshot%20(771).png?raw=true)
![alt text](https://github.com/AmaliJD/Modular-Multiplication-Circles/blob/main/Images/Screenshot%20(775).png?raw=true)
![alt text](https://github.com/AmaliJD/Modular-Multiplication-Circles/blob/main/Images/Screenshot%20(779).png?raw=true)
![alt text](https://github.com/AmaliJD/Modular-Multiplication-Circles/blob/main/Images/Screenshot%20(785).png?raw=true)
![alt text](https://github.com/AmaliJD/Modular-Multiplication-Circles/blob/main/Images/Screenshot%20(786).png?raw=true)

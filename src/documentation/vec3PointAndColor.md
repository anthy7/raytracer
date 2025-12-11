# vec3, point and color

In our program, both points in the 3D world, and color is represented as vectors of size 3.
For points/position, each item in the vector represents one of x, y, z (position along axes).
For colour, each item in the vector represents one of R, G, B (red, green, blue).

## vec3

This is a custom class we have in which 3 doubles are stored. We've overloaded several operators, such as addition, subtraction, multiplication, to allow them to interact with each other.

We can even perform dot, cross products on it. We can retrieve the first, second, and third items with x(), y(), z() respectively.

## point

In vec3.h, we've used 'point3 = vec3' to alias point3 into a vec3. We can specify any x, y, z location to define a point in 3D dimension.

## color

In color.h, we've used 'color' as a kind of alias for vec3. In write_color, we assume that a color can have doubles from 0 to 1, and multiplying and flooring with int() with 255.999 will restrict each field (x,y,z) in vec3 to (0, 255), like they would be RGB.

If we wanted this to be more explicit, we could subclass vec3 into a new class color.

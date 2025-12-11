# ray

Ray tracers have a ray class, which represents 'rays' of light in a 3D scene. A ray may have an origin point, and a direction that it faces. We can calculate further positions by a magnitude given by a 't', that uses the original position and the direction of the ray, and amplifies it depending on the given t. From this, we can later calculate what color is seen at that point on the ray.

## P(t) = A + tb

This is the equation we use to find a position along the ray (beyond the origin)

P -- a 3D position along a line in 3D
A -- ray origin position (vec3/point3)
b -- ray direction (vec3)
t -- a point (double/distance) along the ray.

## Ray class

Defined in ray.h, the ray class contains a position, and a direction. Both are represented as vec3. We can also get the .at(t) of the ray, which uses the equation above to calculate a position at a magnitude t.

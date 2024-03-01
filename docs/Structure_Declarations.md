# Structure Declarations

Structures are used to declare new *types*. Structures are several variables
bundled together into a single package.

We can use structure to represent more complex data types. For example
to represent a point in 2D space we could create a structure called `point`
that packs together two `float` (decimal) values called `x` and `y`. To declare
structures we can use the `struct` keyword in conjunction with the `typedef`
keyword.

typedef struct {
  float x;
  float y;
} point;

We should place this definition above any functions that wish to use it. This
type is no different to the built in types, and we can use it in all the same
ways. To access an individual field we use a dot, followed by the name of the
field, such as `x`.

point p;
p.x = 0.1;
p.y = 10.0;

float length = sqrt(p.x * p.x + p.y * py);

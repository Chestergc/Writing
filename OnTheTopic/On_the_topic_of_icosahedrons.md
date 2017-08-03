# On the topic of Icosahedrons
#### Or how to waste time and still look like you're doing something

Take 4 regular triangles and place them around a shared vertex; the triangles will form a hexagon with a missing triangle in one side, giving that missing triangle's angle missing from the form is equal to sixty.

Taking the triangles placed in an arbitrary place in a plane, with the center able to move in a arbitrary direction perpendicular to said plane, the center starts at 0 in the perpendicular direction

The distance between the points is completely arbitrary, being that they can be any size, according to the starting parameters of the regular triangles used to construct said shape so let the side length be equal to 60.

If you let the center move in a direction perpendicular to the plane, what is the relationship between the height of the center and the angle missing from the hexagon?

Those are simple questions. Why is it that it's never simple to derive a way to calculate things properly?

All that started when we were bored in a 3d modeling class, we were talking about regular polygons and then we decided we wanted to model an icosahedron, but how do you do that?

So, we did the stupid thing first, we started with an octahedron, taking two cubes and intersecting them. Needless to say, it didn't work, getting home right now I've figured out that if I turned the center of every face in to a vertex and connected the dots it would have all worked out pretty well. And it did.

So, how do you start drawing an icosahedron? Well, you can start with a regular pentagon, which is easy to draw in CAD software, displace another one and figure out how to connect the dots so that all the edges are the same length. That bit was easy enough, just take the side of the pentagon, find a plane that goes through both points, draw a point that is the same length away from both points and voilá, you have one of the triangles, do that again around the shape and the main band is done. Now what?

So, how do you get from the center band to the full Icosahedron? That made me go back a couple steps and start thinking about triangles again, simple shapes.

If you take 3 triangles to a vertex and join the edges, they make the top shape of a tetrahedron, pretty simple, intuitive even. Take four, they make a octahedron, a little harder to see, but still there and amazing. Five of them and you get the top portion of an icosahedron. What is the relationship between the angle that is missing from those constructions and the height the vertex needs to get to for those shapes though?

So, for a tetrahedron it is pretty easy to come to the conclusion that the angle to the top is 60 degrees, because it's the angle of the sides of the composing triangles. For the octahedron it's a different story though.

As you can possibly figure out, the dihedral angles on a platonic solid need to be the same in all sides, so if you can measure one of them, the other ones are the same, but, and it's a deal breaker here, how do you measure the angles if you only have the triangles to begin with? You can fit them around an edge and just measure, but that defeats the purpose of the thought experiment, and so I've spend the better part of my evening trying to figure that one out. Haven't even got to the Icosahedron yet.

So, out of the blue, I've came across the formula for the dihedral angle of the icosahedron, given by the formula:

```py
acos(-(sqrt(5)/3))
```

And that completely spoiled the fun. The angle is 138,19 degrees and that is the angle between every face, given that having the same dihedral angle is one of the properties a regular solid must have. Having the angle and the side length of the triangles you can easily compute the end point of the vertex, then mirror it, and fill the gap between them in the same way i've done before. AKA; boring.

The same can be said for the octahedron.

```py
acos(-(1/3))
```

I want to start over. The angle for the octahedron is 109,47 degrees if you're wondering. Start learning maths again, doing it right this time, I can't even consider how the hell would someone even come up with these formulas.

I suppose I will take my time on this one, and make it a good past time, grab a few books on recreational mathematics before diving into the boring stuff they teach in school. There it is, the next topic, recreational mathematics.

#Translation

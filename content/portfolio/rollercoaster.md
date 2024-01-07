+++
showonlyimage = false
draft = false
image = "img/portfolio/a4-paper.jpg"
date = "2023-11-05T18:25:22+05:30"
title = "Roller Coaster Loop Matlab Simulation"
weight = 1
+++

For this project, I created a simulation of a roller coaster loop.
Roller Coaster loops are not perfectly circular due to the amount of force the rider would experience.
I researched what the correct shape is, a clothoid, and modeled it with semi and quarter circles.
<!--more-->

Phase 0 is a cosine wave with the equation 
Phase 1 is a quarter circle with the equation
Phase 2 is a semicircle with the equation
Phase 3 is a quarter circle with the equation
In each phase, I took the equation of the line and then differentiated it twice in order to get the components necessary for the matrix form.
I inputted these equations into this matrix during each phase. This matrix incorporates the constraint equation (the track of the roller coaster that `a` and `b` are based off of, that I differentiated to find in the previous section) and solves for the velocities and accelerations of the cart.
At the end of each phase, I repackage the end conditions of that phase as the start conditions for the next.
B etween phase 1 and 2 and 2 and 3, I had to hardcode in a small “jump” as my differentiation and ODE45 have trouble with those vertical sections.
This graph is a graph of the energy of the system.
As you can see the total energy line is not perfectly flat.
I believe this is due to the fact that I had to make the “jumps” to skip the vertical portions of the loop. It is relatively flat though, and I believe it is enough to validate my system. 
The next thing I wanted to do was optimize for the smallest height of the initial bump that would allow the cart to successfully pass through the loop with my initial conditions (a velocity of `1 m/s` in the x-direction and a cart of 500kgs).
After looping through various heights, it seems 146m is the minimum. This graph shows the speed of the coaster over time.
As you can see, the coaster slows down while in the loop. The maximum speed is 52 m/s, or 116.3 mph, which would make this the 4th fastest roller coaster in the world. The next thing I wanted to test was the forces my riders experience on the ride.
I specifically chose a non circle roller coaster because I wanted to challenge myself and create a coaster that would be safe to ride.
I calculated the acceleration of the cart, and used `𝐹 = 𝑚 * 𝑎` to find the force that the cart experiences.
I then plotted this force over time in newtons and in Gs.
Both plots are in a few segments, which I believe is also due to the jumps I had to make to avoid the verticals. I also added two lines, one at 9 Gs which would kill a passenger, and one at 4 Gs, which would cause the average rider to pass out. To verify this, I also compared my graph's shape to the force over time graph from the paper Roller coasters without differential equations — a Newtonian approach to constrained motion by Rainer Müller in the European Journal of Physics. The graphs
were of similar shape, so I believe this validates my model.

![Video of Final Presentation](https://youtu.be/ucBVkjceUf8)
![Github Repository](https://github.com/oliviajobradley/rollercoasterdynamics)

![Rocky Image][1]
[1]: /img/rocky.jpg
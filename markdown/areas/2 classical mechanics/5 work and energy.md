# Work and Energy

In physics, one of the fundamental laws is that energy must always be conserved in an isolated system. Energy cannot be created or destroyed, only transferred. When energy is transferred, it is capable of doing *work*.

But how does this look in a concrete example?

## Example of Energy

Imagine a ball at the top of a hill.

[img]

At this moment, the ball has some *gravitational potential energy*. This means that it is able to transfer energy from its current height into other things like moving. Gravitational potential energy is calculated as follows:
$$
E_{pg} = mgh
$$
Where $E_{pg}$ is potential gravitational energy, $m$ is mass, and $h$ is height.

Now imagine the ball starts rolling down the hill, which means it is converting its potential energy into *kinetic*, or movement energy. Kinetic energy is calculated as follows:
$$
E_k = \frac{1}{2}mv^2
$$
Where $E_k$ is kinetic energy, $m$ is mass, and $v$ is velocity.

We know that the total energy must remain constant. Therefore, the total energy at the top of the hill and the total energy after having rolled down must be the same. This means we can calculate the velocity it has at the bottom of the hill, using only energy:
$$
\begin{align}
E_{pg} &= E_k \\
mgh &= \frac{1}{2}mv^2 \\
2gh &= v^2 \\
v &= \sqrt{2gh}
\end{align}
$$
This example demonstrates a simple case of energy transfer, as the gravitational potential energy is converted into kinetic energy, but it also demonstrates a simple case of *work* being done. Work is defined as the transfer of energy; Therefore, in this example, work has been done by gravity on the ball, transferring energy to it as it rolls down the hill.

## Work Formula

There is another formula for work:
$$
\begin{align}
W &= F*s&\text{(1 Dimension)} \\
W &= \overrightarrow{F}\cdot\overrightarrow{s}&\text{(2 Dimensions)} \\
W &= |F|*|s|*\cos\theta&\text{(2 Dimensions)}
\end{align}
$$
Where $F$ is force, and $s$ is displacement. In 2 dimensions, it is the dot product of the force vector and the displacement vector.

Let's show how this formula was first found. Imagine pushing a ball along a flat surface. The ball begins at rest with no energy, and pushing it will accelerate it and give it kinetic energy.

[img]

We need to calculate the change in energy, which is the same as work. To do this, we will:

1. Calculate the time that it takes to move a distance $s$.
2. Use this time to get the final velocity of the ball, based on its acceleration.
3. Replace the previous acceleration with the one from $F=ma$.
4. Use the final velocity to get the kinetic energy.

$$
\begin{align}
s &= \underbrace{v_0t}_0 + \frac{at^2}{2} &\to\text{Displacement} \\
t &= \sqrt{\frac{2s}{a}} &\to\text{1. Get time}\\
v &= \underbrace{v_0}_0 + \underbrace{at}_{a\sqrt{\frac{2s}{a}}} &\to\text{2. Get Velocity}\\
v &= \sqrt{2sa} \\
a &= \frac{F}{m} \longrightarrow v = \sqrt{2s\frac{F}{m}} &\to\text{3. Substitute acceleration} \\
E_k &= \frac{1}{2}mv^2 &\to\text{4. Get Kinetic Energy}\\
E_k &= \frac{1}{2}m\left(\sqrt{2s\frac{F}{m}}\right)^2 \\
E_k &= s*F &\to\text{This is the work formula!}
\end{align}
$$

As you can see, in the process of calculating its final energy, we have arrived at the original formula for Work! This means that we can easily use the simple work formula to calculate the *change in energy* of a body being displaced by a force, without having to calculate the energy manually.
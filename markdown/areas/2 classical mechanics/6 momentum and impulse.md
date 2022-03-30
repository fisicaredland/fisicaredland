# Momentum and Impulse

Newton's second law states that objects with more mass are harder to accelerate. *Momentum* is defined as the *quantity of motion*. It depends on mass and velocity, and is commonly symbolized with a $p$:
$$
p = mv
$$
Where $m$ is mass and $v$ is velocity.

Momentum can also be thought of as how *how hard it is to stop a moving object*. If you want to stop a very large boulder from moving, even if it is moving slowly, you need to use a lot of force. Inversely, if you want to stop a baseball shot out of a cannon, even if it is light, you also need a lot of force.

An important property of momentum is that is is *conserved*; The total momentum must remain constant within a closed system. This is useful in many cases to calculate the velocities of bodies before and after a certain event occurs.

But before momentum *really* comes in useful, we also need to understand what *impulse* is. Impulse is a way of quantifying a force that is applied for a certain period of time. It is also equal to the change in momentum, and it is commonly symbolized with a $J$:
$$
\begin{align}
J &= F*t \\
J &= \Delta p
\end{align}
$$
Where $F$ is force and $t$ is time.

## Example 1

Let's say you have a potato cannon, and you shoot a potato out of it.

[img]

You know that the air pressure wave within the cannon pushes the projectile of mass $m$ with a constant force $F$, and you know it takes a time $t$ for the projectile to leave the barrel. How would you calculate the velocity of the projectile after exiting?

One way of calculating this knowing about forces, is to calculate the acceleration and calculate the change in velocity:
$$
\begin{align}
a &= \frac{F}{m} \\
v &= \underbrace{v_0}_0 + at \\
v &= \frac{F}{m}t
\end{align}
$$
But using impulse and momentum, this can be done without involving acceleration:
$$
\begin{align}
J &= F*t \\
p &= mv = F*t \\
v &= \frac{F*t}{m}
\end{align}
$$

## Example 2

Now your potato hits a wall and it gets totally flattened.

If you know that it comes with a momentum of $5\text{ kg*m/s}$ and takes $0.1\text{ s}$ to flatten, how could you calculate the force that was applied on the wall during the collision?

We can just use impulse:
$$
\begin{align}
J &= F*t \\
F &= \frac{J}{t} \\
F &= \frac{5\text{ kg*m/s}}{0.1\text{ s}} \\
F &= 50\text{ N}
\end{align}
$$
So we know that the potato applied a force of 50 newtons into the wall for a tenth of a second.

* As a side note, you may realize that the momentum was not conserved. This is because part of the momentum went into actually moving the wall, part of it went into shooting mashed potato in all directions around the wall, and part of it went into the movement of molecules in the potato, acting as heat.
* This is why you can cook a chicken by only slapping it.
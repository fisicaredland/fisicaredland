# Movement

At its most simple, movement is just a change in position. That means this section will be a lot easier if you know calculus.

## Some basic formulas

$$
\begin{align}
s = \Delta p &= vt\\
\Delta v &= at
\end{align}
$$
Where $s$ and $\Delta p$ are change in position, $\Delta v$ is change in velocity, $a$ is acceleration, and $t$ is time. What this tells us is pretty clear:

- **Velocity** is the change in position over time.
- **Acceleration** is the change in velocity over time.

Easy enough so far. Now, using the above two points, we can do a little calculus to get more formulas:
$$
\begin{align}
v &= v_0 + at \\
p &= p_0 + v_0t + \frac{at^2}{2}
\end{align}
$$
Where $v_0$ is the initial velocity and $p_0$ is the initial position of the system.

## The "highest point in a trajectory" problem

One common physics problem is the projectile following a ballistic trajectory. If we want to know the highest point it reaches, all we need to do is find the point at which the vertical velocity is 0.
$$
\begin{align}
v_y &= v_{0y} + a_yt = 0 \\
t &= \frac{-v_{0y}}{a_y} \\
p_y &= p_{0y} + v_{0y}t + \frac{a_yt^2}{2} \\
p_y &= p_{0y} + v_{0y}\frac{-v_{0y}}{a_y} + \frac{a_y(\frac{-v_{0y}}{a_y})^2}{2} \\
p_y &= p_{0y} - \frac{v_{0y}^2}{a_y} + \frac{v_{0y}^2}{2a_y} \\
p_y &= p_{0y} - \frac{v_{0y}^2}{2a_y}
\end{align}
$$
So we got a formula to calculate the time when the projectile reaches its highest point, and using that, we got a formula to calculate the highest position a projectile will reach. Powerful math.
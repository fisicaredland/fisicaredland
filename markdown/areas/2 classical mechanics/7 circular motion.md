# Circular Motion

Whenever a body moves along a circular path with **constant speed**, its movement is considered *uniform circular motion*.

A common misconception is that spinning objects experience *centrifugal force*, like when you spin around and your arms are pulled outwards, or when you are in a car doing a tight turn and you're pushed towards the outside of the turn. However, there is no such thing as centrifugal force. When you are spinning, your arms try to follow a straight path, but since you are spinning, they appear to move away from you. Equally, when you are in a car that is doing a tight turn, you try to follow the straight path the car had previously, so it appears that you are pushed outwards when in reality you are just following a straight line.

Instead, spinning objects do experience a *centripetal force*: A force pushing the object towards the center of the circumference. The centripetal force is what makes an object follow a curved path when it would otherwise go in a straight line.

There is a simple formula that relates the velocity and mass of an object with its circumference radius and centripetal force:
$$
F_c = m\frac{v^2}{r}
$$
Where $F_c$ is centripetal force, $m$ is mass, $v$ is velocity, and $r$ is radius.

We can also calculate a *centripetal acceleration*, because we know that $F=ma$:
$$
a_c = \frac{v^2}{r}
$$
Where $a_c$ is centripetal acceleration.

## Frequency and period

Another way of defining the velocity of a body moving on a circumference in uniform circular motion is by measuring the number of full turns it covers per unit of time: Its frequency.
$$
f = \frac{n}{\Delta t}
$$
Where $n$ is the number of turns, and $\Delta t$ is the time it takes to cover these turns. Frequency is measured in *oscillations per second*, or hertz.

We can also define a body's velocity based on how long it takes to complete a full turn, the inverse of its frequency. The time it takes for a body to complete a turn of uniform circular movement is called its *period*, and is measured in seconds and symbolized with the letter $T$.
$$
T = \frac{1}{f} = \frac{\Delta t}{n}
$$

## Angular velocity

Now that we have defined frequency and period, we can define angular velocity. Angular velocity is a way of defining an objects velocity depending on how many radians it covers per unit of time. It is symbolized with the letter $\omega$ and is measured in radians per second.

When measuring angles with radians, a full turn is defined as $2\pi$ radians. Therefore, we can easily calculate angular velocity based on frequency or period:
$$
\omega = 2\pi f = \frac{2\pi}{T}
$$
But, what is the purpose of using angular velocity?

It's the same reason we use radians to measure angles instead of degrees: Since a full turn is defined as $2\pi$ radians, and the perimeter of a circle is $2\pi r$, we can easily calculate the perimeter of any arc of a circle based on its angle $\theta$ by just doing $P=\theta r$, but only if the angle $\theta$ is measured in radians.

What this means for uniform circular movement is that we can easily calculate velocity, since the distance covered is an arc:
$$
v = \omega r
$$
As well as centripetal acceleration and force:
$$
\begin{align}
a_c &= \frac{(\omega r)^2}{r} = \omega^2r \\
F_c &= m\omega^2r
\end{align}
$$

## Things to remember

- In any uniform circular movement, the net force **must** point towards the center of the circumference, and be equal to the centripetal force.
- There is no such thing as centrifugal force!
- You can easily convert between tangential velocity and angular velocity by multiplying or dividing by $r$.
- If you know any 2 values in $[a_c,v,r]$, you can calculate the remaining value.
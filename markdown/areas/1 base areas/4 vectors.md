# Vectors

Vectors are an essential component of physics, because we live in a 3-dimensional world (or 4, or 11, or whatever your theories require). In order to describe these kinds of spaces, we have a mathematical object called a vector.

## What is a vector???

I'm sure if you've watched *Despicable Me*, you'll know that Vector commits crimes with "both direction *and* magnitude". And this is how every textbook describes vectors. However, I would like to start explaining them in a way that I think is a bit easier to understand.

At it's most basic, a vector is a *list of numbers*, an array. Specifically, a *1-dimensional matrix*. When you need to describe a 3-dimensional quantity, you use a *3-dimensional vector*, which just means a list of 3 numbers. Vectors look like this:
$$
\overrightarrow{v} = \begin{bmatrix}x\\y\\z\end{bmatrix} = xi+yj+zk
$$
Where $\overrightarrow{v}$ is a vector, $x$, $y$, and $z$ are real numbers, and $i$, $j$, and $k$ are the three unit vectors of the *quaternion number system*. For physics you usually don't need to worry about quaternions unless you're messing with 4 dimensional calculus, so you can just mentally translate any $xi+yj+zk$ you see into $\begin{bmatrix}x\\y\\z\end{bmatrix}$.

Although many say that vectors *have* a direction and a magnitude, these are just properties that *arise from* the vector when applied to a Euclidean space. You can perfectly use vectors purely on paper without ever seeing directions or magnitudes. However, using these to display the vector can help for people who are very visually oriented.

In order to better illustrate vectors, it can help to use an example. Let's say we have a ball at a position $p$, that moves with a velocity $v$. Imagine the ball on the number line. If it begins at $p=0$, it exists at the 0 point on the number line. If its velocity is $1m/s$, it'll move 1 unit to the right each second. Here we can define a basic formula $p=vt$, where t is time. Let's make our ball move to the right at $1m/s$ for $5s$:
$$
\begin{align}
p &= tv \\
p &= 5s*1m/s \\
p &= 5m
\end{align}
$$
We have moved a ball to the right at $1m/s$ for $5s$.

Now imagine this ball exists in a 2-dimensional space. If we wanted to, we could assign a variable for each axis:
$$
\begin{align}
&\left\{\begin{array}{}&p_x = tv_x\\&p_y = tv_y\end{array}\right.\\
&\left\{\begin{array}{}&p_x = 5s*1m/s\\&p_y = 5s*2m/s\end{array}\right.\\
&\left\{\begin{array}{}&p_x = 5m\\&p_y = 10m\end{array}\right.
\end{align}
$$
But this is slow. If we want to go a bit faster, we can just use vectors:
$$
\begin{align}
\overrightarrow{p} &= t\overrightarrow{v} \\
\overrightarrow{p} &= 5s*\begin{bmatrix}1\\2\end{bmatrix}m/s \\
\overrightarrow{p} &= \begin{bmatrix}5\\10\end{bmatrix}m
\end{align}
$$
This is a lot faster. But, in order to use vectors efficiently, we need to know how to combine them.

## Symbology

- A vector is written either $\overrightarrow{v}$ or $\textbf{v}$, depending on the textbook.
- The *magnitude* of a vector is written $|\overrightarrow{v}|$, and is calculated using the Pythagorean theorem, $|\overrightarrow{v}| = \sqrt{v_x^2+v_y^2+v_z^2}$.
- A *unit vector* is a vector whose magnitude equals 1. It is written as $\hat{v}$. You can turn a vector into its unit vector by dividing it in its own magnitude.

## Vector operations

### Addition and subtraction

This one is pretty simple. We just go sideways:
$$
\begin{bmatrix}a\\b\\c\end{bmatrix} + \begin{bmatrix}x\\y\\z\end{bmatrix} = \begin{bmatrix}a+x\\b+y\\c+z\end{bmatrix}
$$

### Multiplication

There are 3 main types of vector multiplication, each with a different use case. The first main one is **scalar multiplication**:
$$
a*\begin{bmatrix}x\\y\\z\end{bmatrix} = \begin{bmatrix}a*x\\a*y\\a*z\end{bmatrix}
$$
Scalar multiplication is used, as the name implies, to multiply a scalar with a vector. This is the multiplication used in the above example with the movement equation.

The next one is the **dot product**:
$$
\begin{align}
\begin{bmatrix}a\\b\\c\end{bmatrix} \cdot \begin{bmatrix}x\\y\\z\end{bmatrix} &= ax+by+cz \\
\begin{bmatrix}a\\b\\c\end{bmatrix} \cdot \begin{bmatrix}x\\y\\z\end{bmatrix} &= \sqrt{a^2+b^2+c^2}*\sqrt{x^2+y^2+z^2}*\cos{\theta}
\end{align}
$$
There are two ways of calculating the dot product. The first way is to multiply sideways and then add all those together, and the second way is to multiply the two magnitudes with the cosine of the angle between the vectors. This identity is mostly used in situations where we want to know the angle, so we can use the first method to get the dot product and then divide that in the two magnitudes to get the cosine of the angle.

The next one is the **cross product**:
$$
\begin{align}
\begin{bmatrix}a\\b\\c\end{bmatrix} \cdot \begin{bmatrix}x\\y\\z\end{bmatrix} &= \begin{bmatrix}bz-cy\\cx-az\\ay-bx\end{bmatrix}\\
\begin{bmatrix}a\\b\\c\end{bmatrix} \cdot \begin{bmatrix}x\\y\\z\end{bmatrix} &= \sqrt{a^2+b^2+c^2}*\sqrt{x^2+y^2+z^2}*\sin{\theta}*\overrightarrow{n}
\end{align}
$$
Where $\overrightarrow{n}$ is a unit vector perpendicular to $\overrightarrow{a}$ and $\overrightarrow{b}$. The cross product is **only defined for 3-dimensional vectors**. This is because it is defined as "$\overrightarrow{a}\cross\overrightarrow{b}$ is a vector perpendicular to both $\overrightarrow{a}$ and $\overrightarrow{b}$". This is applied a lot in electromagnetism.
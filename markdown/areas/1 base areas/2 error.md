# Error

When you take a measurement from an experiment, it is guaranteed to have some form of error. Error sources are classified into the following:

## Error types

### Random error

Random error is, as the name implies, random. It is usually caused by an incomplete control over controlled variables, or other external factors. Randomness also exists within all systems measured, whether it be from temperature, the shifting magnetic field of the Earth, or other sources of noise. Random error is corrected by taking multiple measurements and using statistical techniques to process this data.

### Systematic error

Systematic error, is caused by mistakes in the experimental procedure. This includes instrumental errors, which are caused by incorrect instrument calibration, and other mistakes in the setup of the experiment.

### Measurement error

All instruments have an associated precision and accuracy. If you take a ruler, for example, with marks every millimeter, any measurement you make will only be precise to the nearest millimeter. It is important here to distinguish precision and accuracy:

- **Precision** is the amount that a measurement may vary. Following the example of a ruler with a marking every millimeter, its error can be expressed as $\pm0.5mm$, since the "true" value must be within the range $[x-0.5mm, x+0.5mm]$ for a given measurement $x$.
  - When multiple measurements are taken, the precision of these measurements can be determined using the variance or standard deviation of these measurements.
- **Accuracy** is the closeness between a measurement and the "true" value. Following the example of a ruler with a marking every millimeter, its accuracy will be determined by whether the markings are correctly spaced. If, for example, you measure something to be $10\pm0.5mm$ when the "true" value is $15mm$, this measurement is *precise*, because the variance is low, but not *accurate*, because it is far from the real value.

## Error propagation

https://xkcd.com/2110/

After a value has been measured with an associated error, if we further process this measured value, any mathematical operations we perform using it will also carry with them an error. There is a general formula using partial derivatives that can be used to calculate this; I will not go into explaining this formula here, but I will show its solution for the basic operations.

Considering a function $q = f(x_1,...,x_n)$, the general formula for the error $\Delta q$ is
$$
\Delta q = \sqrt{\sum_{i=1}^n \left(\frac{\part q}{\part x_i}\Delta x_i\right)^2}
$$


### Addition and subtraction

Suppose we want to add values: $(q\pm\Delta q) = (a\pm\Delta a) + (b\pm\Delta b) + ... + (z\pm\Delta z)$.
$$
\begin{align}
q &= a+b+...+z \\
\Delta q &= \sqrt{\Delta a^2 + \Delta b^2 + ... + \Delta z^2}
\end{align}
$$


### Multiplication and division

Suppose we want to multiply values: $(q\pm\Delta q) = (a\pm\Delta a) * (b\pm\Delta b) * ... * (z\pm\Delta z)$.
$$
\begin{align}
q &= a*b*...*z \\
\Delta q &= \sqrt{(\Delta a*(b*c*...*z))^2 + (\Delta b*(a*c*...*z))^2 + ... + (\Delta z*(a*b*...*y))^2} \\
\Delta q &= z\sqrt{\left(\frac{\Delta a}{a}\right)^2 + \left(\frac{\Delta b}{b}\right)^2 + ... + \left(\frac{\Delta z}{z}\right)^2}
\end{align}
$$

### Exponentiation

Suppose we want to exponentiate values: $(q\pm\Delta q) = (a\pm\Delta a)^{(b\pm\Delta b)}$.
$$
\begin{align}
q &= a^b \\
\Delta q &= \sqrt{\left(\Delta a*\frac{a^bb}{a}\right)^2 + (\Delta b*a^b\ln a)^2}
\end{align}
$$

### Single variable functions

Suppose we want to pass $a\pm\Delta a$ into a function $(q\pm\Delta p) = f(a\pm\Delta a)$.
$$
\begin{align}
q &= f(a) \\
\Delta q &= \Delta a * \left|\frac{d}{da}f(a)\right|
\end{align}
$$

## Notes

- Keep in mind that the above formulas apply for errors that are *independent and random*. For instance: If we have a measurement $a=2\pm0.1$, $a-a=0\pm0$; as opposed to $0\pm\sqrt{0.1^2+0.1^2}$.
- If you would like to perform an operation between one variable that has error and one that doesn't, you can just use an error of $\pm0$. $(1\pm0.2) + 1 = (1\pm0.2) + (1\pm0) = 2\pm\sqrt{0.2^2} = 2\pm0.2$.
- **Error is written only with up to 2 significant figures.** This is the kind of thing that they won't forgive you for in a paper. If your result is, for example, $123\pm0.125$, **round it** to $123\pm0.13$.
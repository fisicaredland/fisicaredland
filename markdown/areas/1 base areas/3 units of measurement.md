# Units of Measurement

I'm gonna just ignore the imperial system because it's terrible.

## 7 Base Units

The International System of units of measurement (SI) has 7 base units that all others are derived from:

| **Quantity**              | **Dimension Symbol** | **Unit name** | **Unit symbol** | **Typical symbol (in equations)**       | **Definition**                                               |
| ------------------------- | -------------------- | ------------- | --------------- | --------------------------------------- | ------------------------------------------------------------ |
| Time                      | T                    | Second        | s               | $t$                                     | The duration of $9192631770$ periods of the radiation corresponding to the transition between the two [hyperfine](https://en.wikipedia.org/wiki/Hyperfine_structure) levels of the [ground state](https://en.wikipedia.org/wiki/Ground_state) of the [caesium-133](https://en.wikipedia.org/wiki/Caesium-133) atom. |
| Distance                  | L                    | Metre         | m               | $l$, $h$, $a$, $b$, $x$, $y$, $r$, etc. | The distance travelled by light in a vacuum in $\frac{1}{299792458}$ seconds. |
| Mass                      | M                    | Kilogram      | kg              | $m$                                     | The kilogram is defined by setting the [Planck constant](https://en.wikipedia.org/wiki/Planck_constant) $h$ exactly to $6.62607015*10^{−34} \text{J}\cdot\text{s}$, given the definitions of the metre and the second. |
| Electric current          | I                    | Ampere        | A               | $I$, $i$                                | The flow of exactly $\frac{1}{1.602176634*10^{19}}$ times the [elementary charge](https://en.wikipedia.org/wiki/Elementary_charge) $e$ per second, equalling approximately  $6.2415090744*10^{18}$ elementary charges per second. |
| Thermodynamic Temperature | $\Theta$             | Kelvin        | K               | $T$                                     | The kelvin is defined by setting the fixed numerical value of the [Boltzmann constant](https://en.wikipedia.org/wiki/Boltzmann_constant) $k$ to $1.380649*10^{−23} \text{J}\cdot\text{K}^{−1}$, given the definition of the kilogram, the metre, and the second. |
| Amount of Substance       | N                    | Mole          | mol             | $n$                                     | The amount of substance of exactly $6.02214076*10^{23}$ elementary entities. This number is the fixed numerical value of the [Avogadro constant](https://en.wikipedia.org/wiki/Avogadro_constant), $N_A$, when expressed in the unit $\text{mol}^{−1}$. |
| Luminous Intensity        | J                    | Candela       | cd              | $I_v$                                   | The luminous intensity, in a given direction, of a source that emits monochromatic radiation of frequency $5.4*10^{14}$ hertz and that has a radiant intensity in that direction of $\frac{1}{683}$ watt per [steradian](https://en.wikipedia.org/wiki/Steradian). |

All other units of measurement in the SI are derived from combinations of these. For example:

- Velocity is a measurement of length over time: $\frac{\text{length}}{\text{time}} = \frac{m}{s} \to m/s$.
- Acceleration is a measurement of velocity over time: $\frac{\text{velocity}}{\text{time}} = \frac{m/s}{s} \to m/s^2$.
- Force is a measurement of mass times acceleration: $\text{mass}*\text{acceleration} = m*m/s^2 \to m^2/s^2 = N$.

This means that for any calculation, if you just transform the units correctly, you can know the exact unit of the result, which can be described by its *basic unit dimensions* which are a combination of the main 7 units.

## Derived Units

Here is a basic table of the most common units and their basic unit dimensions:

| Name                                                         | Symbol | Quantity                                                     | In SI base units                                | In other SI units |
| ------------------------------------------------------------ | ------ | ------------------------------------------------------------ | ----------------------------------------------- | ----------------- |
| **[radian](https://en.wikipedia.org/wiki/Radian)**           | rad    | [plane angle](https://en.wikipedia.org/wiki/Angle)           | $\text{m}/\text{m}$                             | 1                 |
| **[steradian](https://en.wikipedia.org/wiki/Steradian)[[N 1\]](https://en.wikipedia.org/wiki/International_System_of_Units#cite_note-:0-129)** | sr     | [solid angle](https://en.wikipedia.org/wiki/Solid_angle)     | $\text{m}^2/\text{m}^2$                         | 1                 |
| **[hertz](https://en.wikipedia.org/wiki/Hertz)**             | Hz     | [frequency](https://en.wikipedia.org/wiki/Frequency)         | $\text{s}^{−1}$                                 |                   |
| **[newton](https://en.wikipedia.org/wiki/Newton_(unit))**    | N      | [force](https://en.wikipedia.org/wiki/Force), [weight](https://en.wikipedia.org/wiki/Weight) | $\text{kg}\cdot\text{m}\cdot\text{s}^{−2}$      |                   |
| **[pascal](https://en.wikipedia.org/wiki/Pascal_(unit))**    | Pa     | [pressure](https://en.wikipedia.org/wiki/Pressure), [stress](https://en.wikipedia.org/wiki/Stress_(physics)) | $\text{kg}\cdot\text{m}^{−1}\cdot\text{s}^{−2}$ | $\text{N}/\text{m}^2$ |
| **[joule](https://en.wikipedia.org/wiki/Joule)**             | J      | [energy](https://en.wikipedia.org/wiki/Energy), [work](https://en.wikipedia.org/wiki/Mechanical_work), [heat](https://en.wikipedia.org/wiki/Heat) | $\text{kg}\cdot\text{m}^2\cdot\text{s}^{−2}$           | $\text{N}\cdot\text{m} = \text{Pa}\cdot\text{m}^3$ |
| **[watt](https://en.wikipedia.org/wiki/Watt)**               | W      | [power](https://en.wikipedia.org/wiki/Power_(physics)), [radiant flux](https://en.wikipedia.org/wiki/Radiant_flux) | $\text{kg}\cdot\text{m}^2\cdot\text{s}^{−3}$            | $\text{J}/\text{s}$ |
| **[coulomb](https://en.wikipedia.org/wiki/Coulomb)**         | C      | [electric charge](https://en.wikipedia.org/wiki/Electric_charge) | $\text{s}\cdot\text{A}$                             |                   |
| **[volt](https://en.wikipedia.org/wiki/Volt)**               | V      | [electrical potential difference](https://en.wikipedia.org/wiki/Electrical_potential_difference) ([voltage](https://en.wikipedia.org/wiki/Voltage)), [emf](https://en.wikipedia.org/wiki/Electromotive_force) | $\text{kg}\cdot\text{m}^2\cdot\text{s}^{−3}\cdot\text{A}^{−1}$ | $\text{W}/\text{A} = \text{J}/\text{C}$ |
| **[farad](https://en.wikipedia.org/wiki/Farad)**             | F      | [capacitance](https://en.wikipedia.org/wiki/Capacitance)     | $\text{kg}^{−1}\cdot\text{m}^{−2}\cdot\text{s}^4\cdot\text{A}^2$ | $\text{C}/\text{V} = \text{C}^2/\text{J}$ |
| **[ohm](https://en.wikipedia.org/wiki/Ohm_(unit))**          | Ω      | [resistance](https://en.wikipedia.org/wiki/Electrical_resistance), [impedance](https://en.wikipedia.org/wiki/Electrical_impedance), [reactance](https://en.wikipedia.org/wiki/Reactance_(electronics)) | $\text{kg}\cdot\text{m}^2\cdot\text{s}^{−3}\cdot\text{A}^{−2}$ | $\text{V}/\text{A} = \text{J}\cdot\text{s}/\text{C}^2$ |
| **[siemens](https://en.wikipedia.org/wiki/Siemens_(unit))**  | S      | [electrical conductance](https://en.wikipedia.org/wiki/Electrical_conductance) | $\text{kg}^{−1}\cdot\text{m}^{−2}\cdot\text{s}^3\cdot\text{A}^2$ | $\Omega^{−1}$    |
| **[weber](https://en.wikipedia.org/wiki/Weber_(unit))**      | Wb     | [magnetic flux](https://en.wikipedia.org/wiki/Magnetic_flux) | $\text{kg}\cdot\text{m}^2\cdot\text{s}^{−2}\cdot\text{A}^{−1}$ | $\text{V}\cdot\text{s}$ |
| **[tesla](https://en.wikipedia.org/wiki/Tesla_(unit))**      | T      | [magnetic flux density](https://en.wikipedia.org/wiki/Magnetic_flux_density) | $\text{kg}\cdot\text{s}^{−2}\cdot\text{A}^{−1}$         | $\text{Wb}/\text{m}^2$ |
| **[henry](https://en.wikipedia.org/wiki/Henry_(unit))**      | H      | [inductance](https://en.wikipedia.org/wiki/Inductance)       | $\text{kg}\cdot\text{m}^2\cdot\text{s}^{−2}\cdot\text{A}^{−2}$ | $\text{Wb}/\text{A}$ |
| **[degree Celsius](https://en.wikipedia.org/wiki/Degree_Celsius)** | °C     | [temperature](https://en.wikipedia.org/wiki/Temperature) relative to $273.15\text{K}$ | $\text{K}$                                      |                   |
| **[lumen](https://en.wikipedia.org/wiki/Lumen_(unit))**      | lm     | [luminous flux](https://en.wikipedia.org/wiki/Luminous_flux) | $\text{cd}\cdot\text{sr}$                          | $\text{cd}\cdot\text{sr}$ |
| **[lux](https://en.wikipedia.org/wiki/Lux)**                 | lx     | [illuminance](https://en.wikipedia.org/wiki/Illuminance)     | $\text{cd}\cdot\text{sr}\cdot\text{m}^{−2}$      | $\text{lm}/\text{m}^2$ |
| **[becquerel](https://en.wikipedia.org/wiki/Becquerel)**     | Bq     | [activity referred to a radionuclide](https://en.wikipedia.org/wiki/Radioactive_decay) (decays per unit time) | $\text{s}^{−1}$                                 |                   |
| **[gray](https://en.wikipedia.org/wiki/Gray_(unit))**        | Gy     | [absorbed dose](https://en.wikipedia.org/wiki/Absorbed_dose) (of [ionising radiation](https://en.wikipedia.org/wiki/Ionising_radiation)) | $\text{m}^2\cdot\text{s}^{−2}$                      | $\text{J}/\text{kg}$ |
| **[sievert](https://en.wikipedia.org/wiki/Sievert)**         | Sv     | [equivalent dose](https://en.wikipedia.org/wiki/Equivalent_dose) (of [ionising radiation](https://en.wikipedia.org/wiki/Ionising_radiation)) | $\text{m}^2\cdot\text{s}^{−2}$                      | $\text{J}/\text{kg}$ |
| **[katal](https://en.wikipedia.org/wiki/Katal)**             | kat    | [catalytic activity](https://en.wikipedia.org/wiki/Catalytic_activity) | $\text{mol}\cdot\text{s}^{−1}$                     |                   |

## Prefixes

All SI units can be prefixed with any of the following prefixes to multiply them by a power of 10.

| **Prefix**                                    | **Symbol** | **Base 10** |
| --------------------------------------------- | ---------- | ----------- |
| [yotta](https://en.wikipedia.org/wiki/Yotta-) | Y          | $10^{24}$   |
| [zetta](https://en.wikipedia.org/wiki/Zetta-) | Z          | $10^{21}$   |
| [exa](https://en.wikipedia.org/wiki/Exa-)     | E          | $10^{18}$   |
| [peta](https://en.wikipedia.org/wiki/Peta-)   | P          | $10^{15}$   |
| [tera](https://en.wikipedia.org/wiki/Tera-)   | T          | $10^{12}$   |
| [giga](https://en.wikipedia.org/wiki/Giga-)   | G          | $10^9$      |
| [mega](https://en.wikipedia.org/wiki/Mega-)   | M          | $10^6$      |
| [kilo](https://en.wikipedia.org/wiki/Kilo-)   | k          | $10^3$      |
| [hecto](https://en.wikipedia.org/wiki/Hecto-) | h          | $10^2$      |
| [deca](https://en.wikipedia.org/wiki/Deca-)   | da         | $10^1$      |
|                                               |            | $10^0$      |
| [deci](https://en.wikipedia.org/wiki/Deci-)   | d          | $10^{-1}$   |
| [centi](https://en.wikipedia.org/wiki/Centi-) | c          | $10^{-2}$   |
| [milli](https://en.wikipedia.org/wiki/Milli-) | m          | $10^{-3}$   |
| [micro](https://en.wikipedia.org/wiki/Micro-) | μ          | $10^{-6}$   |
| [nano](https://en.wikipedia.org/wiki/Nano-)   | n          | $10^{-9}$   |
| [pico](https://en.wikipedia.org/wiki/Pico-)   | p          | $10^{-12}$  |
| [femto](https://en.wikipedia.org/wiki/Femto-) | f          | $10^{-15}$  |
| [atto](https://en.wikipedia.org/wiki/Atto-)   | a          | $10^{-18}$  |
| [zepto](https://en.wikipedia.org/wiki/Zepto-) | z          | $10^{-21}$  |
| [yocto](https://en.wikipedia.org/wiki/Yocto-) | y          | $10^{-24}$  |


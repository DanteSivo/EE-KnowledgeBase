# Math Concepts
## Complex Forms
Electrical values are often expressed in non-rectangular fields. This is most commonly found in the use of **complex current**. This section will go over the forms commonly used and how to convert between them.

![](images\xyz-graph.jpg){ width="300" }

 For instance

$$
\begin{equation}
\overline{Z} = X + jY
\end{equation}
$$
Where X is the real part of Z

And Y is the complex part of Z

### Rectangular Form
The standard coordinate field from elementrary school. Fields are orinated in the X, Y, and Z fields. 

### Polar Form
Standard use for complex numbers in engineering applications. Aka **exponential form**

$$
\begin{equation}
    \overline{Z} = Z \cdot{} e^{j\theta{}} = Z \angle \theta{}
\end{equation}
$$

Note that $\theta$ must be in radians. In terms of rectangular, $\theta$ is the angle between the real and complex components of $\overline{Z}$.

==Rectangular to Polar==
$$
\begin{equation}
    Z = \sqrt{X^2 + Y^2}
    \\
    \theta = \arctan(Y/X)
\end{equation}
$$
==Polar to Rectangular==
$$
\begin{equation}
    X = Z \cdot cos(\theta)
    \\
    Y = Z \cdot sin(\theta)
\end{equation}
$$
### Cylindrical Form
From E&M Fields & Transmission Lines.
### Spherical Form
From E&M Fields & Transmission Lines.
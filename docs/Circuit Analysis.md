# Circuit Analysis
Documentation for basic circuit analysis techniques that can be used in all circuits

## Kirchhoff's Voltage Law (KVL)

==The voltage into and out of any given node is zero==
$$
\begin{equation}
    \Sigma{V} = 0
\end{equation}
$$

![](images\KVL_Circuit.jpg){ width="300" }

## Kirchhoff's Current Law (KCL)

==The amount of current entering and exiting a node is equal==
![](images\KCL_Circuit.gif){ width="400" }

## Circuit Simulators
### FALSTAD 
An [Online Simulator](https://www.falstad.com/circuit/) that demonstrates the current flow of a specified electrical signal in an animated format.
 
![](images\FALSTAD-GIF.gif)

**NOTE** - FALSTAD is **NOT** SPICE based. This means that while the components in FALSTAD are closely coorilated to SPICE, they are not 1 to 1. 
### SPICE

AKA Simulation Program with Integrated Circuit Emphasis. First developed in the 70s, SPICE has evolved into the primary circuit simulation software world wide. Highly configurable with detailed settings. [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is a common light-weight program used around the world.

## Mesh Analysis
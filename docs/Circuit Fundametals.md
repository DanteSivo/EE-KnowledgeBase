# Circuit Fundamentals
This section will go over the various basics of electronics and associated fields

## What is a Circuit?
**Electronic Circuit** - Any device that performs characterisitcs associated with the movement of electrons
> Ex: Static Shocks, Home Wiring, Light up Toys, etc.

A circuit can be generally considered to have 3 parts.

1. **Electron Source** - This "powers" the circuit
2. **Intermediate Devices** - Filters, IC's, anything that isn't in any other category
3. **Load** - The primary recipiant of the Electron Source. Usually an IC or a passive load.

pages:
- Home: 'index.md'
- About: 'about.md'

## Definition of Current
**Conventional Current** - Direction of curent flow used for analysis

**Electron Flow** - Direction of electron flow (opposite of Conventional Current)
  
Trivia: This is because Ben Franklin took a coin flip to decide the direction of current and was wrong. Oh well.  

![](images\current-electron-conventional-flow-01.svg)


**Current** - The flow of electrons through a conductor

Current flow induces the following

1. **Heat** - More thermal disipation at higher currents and resistances. 
   The amount of energy disipated as heat is defined as H. Where H is the amount of heat disipated in Joules, I in Amps, R in Ohms, and t is time. 
$$
\begin{equation}
    H = I^2Rt
\end{equation}
$$
2. **EMF Field** - A conductor will build up a magnetic field, effictivley acting like an inductor.

## Circuit Simulators
### FALSTAD 
An [Online Simulator](https://www.falstad.com/circuit/) that demonstrates the current flow of a specified electrical signal in an animated format.
 
![](images\FALSTAD-GIF.gif)

**NOTE** - FALSTAD is **NOT** SPICE based. This means that while the components in FALSTAD are closely coorilated to SPICE, they are not 1 to 1. 
### SPICE

AKA Simulation Program with Integrated Circuit Emphasis. First developed in the 70s, SPICE has evolved into the primary circuit simulation software world wide. Highly configurable with detailed settings. [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html) is a common light-weight program used around the world.

## What is a Volt?
$$
\begin{equation}
    V = \dfrac{potential\ energy}{charge} = \dfrac{J}{C} = \dfrac{kg\cdot{}m^2\cdot{}s^{-2}}{A\cdot{}s}
\end{equation}
$$

Through Ohm's Law. We know that...

$$
\begin{equation}
    V = A\cdot{}\Omega=\dfrac{Wb}{s} = \dfrac{W}{A} = \dfrac{J}{C} = \dfrac{eV}{e}
\end{equation}
$$

Note, Wb is webers per second (magnetic flux per time).

Volts is also **power per current** or **energy per charge**

The **higher** your voltage, the more electromotive force is generated. This is because...
$$
\begin{equation}
    E = V + IR
\end{equation}
$$
Where R is the internal resistance of the motor. So **for no internal resistance, Electromotive Force is correlated to Voltage**
# Circuit Devices
Documentation for all standard components. Specific components that can be generalized with similar characteristics are grouped together. (Ex. Schottky  Diode is with Diodes).

## Resistor

The simplest of all electrical components. A resistor is a *passive* two terminal device that applies electrical resistance. *Temperature does affect resistance*

### Thick Film Resistor
Standard THT resistor commonly found in prototypes around the world. 
```
+ Cheap and Easy to work with
+ Various packages for different amounts of power dissipation
- Low Tolerance, package leads adjust resistance slightly
- Stray Capacitance, package lengths add in line capacitance
``` 
![](images\thick-film-resistors.jpg){ width="300" }

### Potentiometer
Adjustable resistance based either on a physical knob or a digital register. Adjustable between two resistance values. Can be either THT or SMD.

## Capacitor

Stores electrical charge in an electric field. 

Two conductive plates are seperated by a dielectric to store charge.  ![](images/ParallelCapcitorModel.png)

The capacitance is defined as 
$$
\begin{equation}
    C = \dfrac{Q}{V} = \dfrac{\epsilon{}\cdot{}A}{d}
\end{equation}
$$ 
## Induct

## Diodes

## MOSFET 
Stands for Metal-Oxide-Semiconductor-Field-Effect transistor

## BJT (Bipolar Junction Transistor)
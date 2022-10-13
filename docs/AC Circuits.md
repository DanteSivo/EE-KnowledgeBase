# AC Circuits

Circuits where the core functionality of the device is based on Alternating Current (AC) principles.

## RC Time Constant

A capacitor in series with a transmission line will take some time to charge. 

* For a DC Circuit, charged capacitors act like a wire
* For a AC Circuit, capacitors are considered open until charged.

$RC$  is considered the *time constant* $\tau{}$

$$
\tau{} = R \cdot{} C
$$

==Charging Equation== - Voltage on capacitor while accumulating current
$$
\begin{equation}
v(t) = v_o \cdot{} (1-e^{\dfrac{-t}{RC}})
\end{equation}
$$
![](images/RC-ChargingSim.JPG){width: "400"}
SPICE Sim -> [Click to Download](SPICE-files/RC-Charging.asc)

==Discharging Equation== - Voltage on capacitor while discharging current
$$
\begin{equation}
v(t) = v_o \cdot{} e^{\dfrac{-t}{RC}}
\end{equation}
$$
![](images/RC-DischargingSim.JPG){width: "400"}
SPICE Sim -> [Click to Download](SPICE-files/RC-Discharging.asc)
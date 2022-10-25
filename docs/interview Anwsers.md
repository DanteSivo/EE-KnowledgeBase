# Interview Anwsers

## Basic Questions

1. **What is the Equation of a Voltage Divider?**

2. **What is the definition of Capacitance?**

3. **How does a FPGA differ from a Microprocessor?**

4. **How do ADC's work?**

5. **What is the point of impedance matching?**

6. **How does a BJT work?**

7. **How does a MOSFET work?**

8. **How does an H-Bridge work?**

## Boolean Alegbra
### Simplifiy The Boolean Expression
$$ \overline{A}CC + \overline{A}BC + A\overline{B}\overline{C} + A\overline{B}C = \overline{A}BC + A\overline{B} $$

## Digital Logic
### SR Latch

## BJTs
1. **Determine $I_C$, $I_B$, $I_E$ and $V_C$, $V_B$, $V_E$**
    ![](images\bjt-question-1.JPG){ width="600" } 
    Assuming the BJT is in Active Mode, $V_{BE} = 0.7(v)$
    $$ 
    \begin{equation}
    V_{BE} = V_B - V_E = 0.7
    \\
    I_C = \beta{}I_{B} = 99I_B 
    \end{equation}
    $$

    Taking KVL from B-E
    $$ 
    \begin{equation}
    V_{sig} = R_B I_B - V_{BE} - R_E I_E = 0
    \\
    5.7(v) - (10k\Omega{})I_B - 0.7(V) - (2k\Omega{})(\beta{}+1)(I_B)= 0
    \\
    \boxed{I_B = 23.8uA}
    \\
    I_C = \beta{}I_B = \boxed{2.356mA = I_C}
    \\
    I_E = (\beta{} + 1)I_B = \boxed{2.380mA = I_E}
    \\
    V_C = V_{CC} - I_C(R_C) = 10.7 - (2.356mA)(1k\Omega{}) = \boxed{8.34(V) = V_C}
    \\
    V_E = V_C - V_E = \boxed{3.58(V) = V_E}
    \end{equation}
    $$

    Take KVL from C-E
    $$
    \begin{equation}
    V_{sig} - I_C R_C - V_{CE} - I_E(R_E) = 0
    \\
    \boxed{V_{CE} = 3.58(V)}
    \\ V_{CE} = V_{CE} + V_{BE} = \boxed{2.88(V) = V_{CE}}
    \end{equation}
    $$

    ==Check that Assumption of Operating Mode is correct==
    $$
    \begin{equation}
    V_{CE} > 0.7(V) \checkmark
    \\
    I_B > 0 \checkmark
    \end{equation}
    $$

2. **Determine $I_C$ and $V_C$**



## Op-Amp
1. **What does Op-Amp stand for?**
2. 

## RC Circuits
1. **Sketch the output given the input for the two circuits.**

    ![](images\RC-Circuits-A1.JPG){ width="600" } 

    SPICE Sim R//C//R -> [Click to Download](SPICE-files/RC-Circuits-A1_1.asc)

    SPICE Sim C//R//C -> [Click to Download](SPICE-files/RC-Circuits-A1_2.asc)

    [YouTube explaination](https://www.youtube.com/watch?v=1N99I_Z1YQc)

2. **Given the circuit starts open, when SW1 closes. What is the voltage accross C1 and C2?**

    ![](images\RC-Circuits-Q2.JPG){ width="600"}

    C1 will reach the same voltage as the input voltage after it has been completley charged. This time can be determined through the use of the equation 
    $V = Vo \cdot{} e^{-t/(RC)}$ where $t$ is determined. Since C2 is not connected to the voltage source, it remains at 0V.

    **Now, SW1 opens and SW2 closes. What is the voltage across C1 and C2 given SW1 has been closed for a long time?**

    When SW2 is closed, the voltage on C1 is equal to 5V and the voltage on C2 is 0V. Because of the potential difference, current will flow from C1 to C2 until the potential difference is 0. To determine the final voltage, the total capacitance should be considered.

    $$ 
    \begin{equation}
    Ceff = C1 + C2 = 2C
    \\
    C = \dfrac{Q}{\Delta{}V} 
    \end{equation}
    $$

    Given C1 is charged, we know the total charge on C1 is $Q_1 = C_1 \cdot{} \Delta{}V_1$
    In order to **conserve charge**, $Q_{eff}$ must equal $Q_1$. ==The amount of charge cannot change.==

    $$ 
    \begin{equation}
        Q_1 = C_{eff} \cdot{} \Delta{}V_{eff}
    \\
        C_1(V_1) = (C_1 + C_2) \cdot \Delta{}V_{eff}
    \\ 
        \dfrac{C_1(V_1)}{C_1 + C_2} = \Delta{}V_{eff}
    \end{equation}
    $$

    Therefore, the voltage on C1 and C2 will be equal at some value less than 5V.
    
3. **When SW1 closes what is Vout?**

    ![](images\RC-Circuits-Q3.JPG){ width="500"}

    ==Convservation of Charge== 
    
    The current through C2 is the same going through C1. So the charge on $q_1 = q_2$. 

    The definition of the total charge on a capacitor is $q = c \cdot{} \Delta{}v$

    $$
        \begin{equation}
            \Delta{} V_2 = V_{in} - V_{out}
            \\
            \Delta{} V_1 = V_{out} - 0
            \\
            C_2\Delta{}V_2 = C_1\Delta{}V_1
            \\
            4C(V_{in} - V_{out}) = C(V_{out} - 0)
            \\
            4(5V - V_{out}) = V_{out}
            \\
            V_{out} = \dfrac{20V}{5} = 4V 
        \end{equation}
    $$
## Advanced Examples

### Switch Mode Power Supply
# PCB Tips

This page will document various tips and tricks for PCB development, along with some long standing concepts and theories.

## Decoupling Capacitors

To eliminate AC ripple, a small capacitor is generally placed near the power input of an IC (integrated-circuit).

The distance between the capacitor and the terminal desitination needs to be **as small as possible**. This reduces the line inductance which can make a huge difference.

    Ex). Putting a cap 12 inches away results in a line inductance of 240nH.
         Placing it to within an inch lowers it to 20nH.

[More information](http://www.interfacebus.com/Design_Capacitors.html) 
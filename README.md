![schematic.js example](https://raw.githubusercontent.com/PelleJuul/schematic.js/master/misc/example.png)
# schematic.js
A JavaScript library for embedding electrical ciruit schematics in webpages. Provides a set of functions to draw common schmatic elements such as resistors, capacitors, wires, and so on.

Until we get an actual API documentation, take a look a the source code to see how to use *schematic.js* (the source code is not very long).

## Domain Specific Language
In the future *schematic.js* will also include a domain specific language for easy construction of schematics. This language should be easy to embed into webpages, such that no JavaScript is required to draw schematics. Maybe it could look something like

```html
<x-schematic>
terminal (1, 1) "Input"
resistor (1, 1) (5, 1)
joint (5, 1)
capacitor (5,1) (5, 4)
ground (5, 4)
wire (5, 1) (8, 1)
terminal (8, 1) "Output"
</x-schematic>
```

This should draw the example schematic seen at the top of this document. 

## Contributing
Contributing to schematic.js is very easy. Right now the main focus is to create draw rutines for common electrical components. Some suggestions:

- [ ] Batteries
- [x] Capacitors, non-polarized
- [ ] Capacitors, polarized
- [ ] Connectors (coaxial, jack)
- [ ] Crystals
- [ ] DC sources (Vcc, Vdd)
- [ ] Diodes (normal, zener, schottky)
- [ ] Generics ICs
- [x] Ground
- [ ] LEDs
- [ ] Logic gates
- [ ] Meters (voltage, ampere)
- [ ] Op-amps
- [x] Resistors
- [ ] Switches
- [x] Terminals
- [ ] Transistors (PNP, NPN, JET, MOSFET)
- [x] Wires

Take a look at the sources code to get a feel for how the draw functions should look like.

# Wokwi cd4070b Chip

This is a custom chip for [Wokwi](https://wokwi.com/). It implements the cd4070b IC.

## Description

The cd4070b contain faur independent 2-input Exclusive-OR gates. Each gate performs the Boolean function
of j = A ⊕ B (for gate 1 in this case) in positive logic.

## Truth Table (1 for each gate)


| INPUT A | INPUT B |  OUTPUT |
|---------|---------|---------|
|    L    |    L    |    L    | pass
|    H    |    L    |    H    | pass
|    L    |    H    |    H    | pass
|    H    |    H    |    L    |

## Pin names

| Name | Description       |
| ---- | ----------------- |
|  A   | Input signal  A   |
|  B   | Input signal  B   |
|  J   | Gate 1Output signal   |
|  C   | Input signal  C   |
|  D   | Input signal  D   |
|  K   | Gate 1Output signal   |
|  E   | Input signal  E   |
|  F   | Input signal  F   |
|  L   | Gate 1Output signal   |
|  G   | Input signal  G   |
|  H   | Input signal  H   |
|  M   | Gate 1Output signal   |
| GND  | Ground            |
| VCC  | Supply voltage    |


## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-cd4070b": "github:wokwi-custom-chips/cd4070b@0.1.0"
  }
```

Then, add the chip to your circuit by adding a `chip-cd4070b` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "chip-cd4070b", "id": "chip1" }
  },
```

For a complete example, see [The cd4070b chip test project](https://wokwi.com/projects/398983628077680641).

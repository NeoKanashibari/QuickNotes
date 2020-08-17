# HUION - Tablet graphic

# Available Drivers

1. https://github.com/konachan700/Q11K_Driver
2. https://github.com/DIGImend/digimend-kernel-drivers.git

Prefers the from DIGImend.

## Mapping tablet to screen
```sh
xsetwacom set HUION Huion Tablet Pen stylus MapToOutput DP-2
```

## Tablet Pressure
```sh
xsetwacom set "HUION Huion Tablet Pen stylus" PressureCurve <values>
```
### available values are:
  0 100   0 100  # ridiculously soft
  0  50  50 100  # very soft
  0   0 100 100  # linear, the default
 50   0 100  50  # very firm
100   0 100   0  # unbelievably firm

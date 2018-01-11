# 19F qNMR
- Chemical shifts: 5-fluorouracil (-170 ppm, s or brd), sodium fluoride (-125.8 ppm, s), fluoroacetate (-217.86 ppm, t), fluorothreonine (-231.6 ppm, dt) 
- Center the measurement: `o1p = N`, N = chemical shift of the molecule.
- Determine the 90 degree pulze (p1 value). Final parameters: `p1 = 7`, `p2 = 14`.
- Determine the T1 value. *Note: This step can be skipped. Directly use `d1 = 25 s`, which should cover most organofluorines. For 5-fluorouracil, I used `d1 = 20 s` to save instrument time.*
- Collect data for each molecule (4 measurements each sameple) using parameters: `p1 = 7`, `p2 = 14`, `o1p = N`, `rg = 128`, `d1 = 20 s or 25 s`, `ns = 8`, `td0 = 1` (`td0 = 3` for fluorothreonine). 

## To begin measurement
- **VT**: `edte` target T 298 K, Max heating 3%, gas flow 800 L/h, clink heat on, monitor the temperature.
- **Change the cables**: unscrew both green and yellow cables, and then screw the yellow cable into the green plug. Basically move the top cable down one position. The filter on the green cable has to be removed as well. 

## 90 degree pulse measurement

- `new`, `rpar` -> search for \*19\*

## T1 measurement




- **VT off**: `edte` turn off heater, *confiqure* -> click load config -> VT_off to reset the default setting
- **Switch the cables back**
- load 1H parameter by clicking rpar, `atma` -> tune back to proton channel
- `lock` and then `topshim gui`.
- put standard tube back, `user`, log off.

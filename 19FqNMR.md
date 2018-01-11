# 19F qNMR
- Chemical shifts: 5-fluorouracil (-170 ppm) reference (C0) and analytes (C1, C2 ...). 
- Center the window on Cn by `o1p=Cn`.
- Determine the 90 degree pulze (p1 value).
- Determine the T1 value. *Note: This step can be skipped. We can directly use `d1=25s`, which should cover most organofluorines.*
- Collect data for Cn using consistent parameters: `p1`, `p2`, `o1p=Cn`, `rg`, `d1=25s`, `ns`, `td0`. 
- Then collect data for C1, C2 ....

## To begin
- **VT**: `edte` target T 298 K, Max heating 3%, gas flow 800 L/h, clink heat on, monitor the temperature.
- **Change the cables**: unscrew both green and yellow cables, and then screw the yellow cable into the green plug. Basically move the top cable down one position. The filter on the green cable has to be removed as well. 

## 90 degree pulse measurement

- `new`, `rpar` -> search for \*19\*

## T1 measurement




- **VT off**: `edte` turn off heater, *confiqure* -> click load config -> VT_off to reset the default setting
- **Switch the cables back**
- load 1H parameter, `atma` -> tune back to proton channel
- put standard tube back, `user`, log off.

# Atmospheric Model
I recalculated the 1976 atmospheric model in higher accuracy and saved it as a CSV.
I calculated the values from -5km to 1000km in steps of 50 m for maximum accuracy, you can calculate it as well by using using the equations:
```math
g = G \frac{{m_0}}{{(6378137 + h_0)^2}}
```
```math
p = \exp\left(-\frac{g}{RT} \times h_1\right) \times 101325
```
__Gravitational Force Equation__
<br/>
G is the gravitional constant (N⋅m2/kg2) = 6.67430e−11 N⋅m2/kg2
<br/>
m0 is the mass of Earth (kg) = 5.9722e+24 kg
<br/>
h0 is the altitude above sea level (metres)

__Pressure Equation__
<br/>
g is the gravitional acceleration (m/s) = 9.80665m/s or the equation provided
<br/>
R is the gas constant (kJ⋅kg−1⋅K−1) = 0.287052874 kJ⋅kg−1⋅K−1
<br/>
h1 is the altitude above sea level (kilometres)
<br/>
p is the atmospheric pressure (pascals)
<br/>
T is the absolute temperature (K) = Check lookup table, lerp between the points
| Altitude (m) | Temperature (K) |
| ------------- | ------------- |
| -5000  | 320.676 |
| 0  | 288.15  |
| 11000  | 216.65 |
| 20000  | 216.65  |
| 32000  | 228.65 |
| 47000  | 270.65  |
| 51000  | 270.65 |
| 71000  | 214.65  |
| 86000  | 187.15 |
| 815000  | 1000  |

__Sources__
<br/>
Gas Constant Value: https://en.wikipedia.org/wiki/Gas_constant
<br/>
Reference: https://www.ngdc.noaa.gov/stp/space-weather/online-publications/miscellaneous/us-standard-atmosphere-1976/us-standard-atmosphere_st76-1562_noaa.pdf
<br/>
Theory: https://www.robertribando.com/wp-content/uploads/2022/08/USStandardAtmosphere.pptx
<br/>
US Standard Atmosphere: https://en.wikipedia.org/wiki/U.S._Standard_Atmosphere
<br/>
Data Points: https://en.wikipedia.org/wiki/U.S._Standard_Atmosphere
<br/>
<br/>
<br/>
Hope you found this useful!

# Simulation of the Relativistic Doppler Shift Effect

This project simulates the relativistic Doppler effect by transforming images according to

\$\$ \lambda' = \frac{\lambda}{\gamma (1 - \beta \cos\theta)} \$\$ 

where:
- \(\lambda'\): Transformed wavelength  
- \(\lambda\): Original wavelength  
- \(\beta = v/c\): Velocity as a fraction of the speed of light  
- \(\theta\): Angle of view
- gamma: The lorentz factor


## Examples
```python
transform_image(file="example.jpg", beta=-0.15, angle_of_view=np.radians(38))


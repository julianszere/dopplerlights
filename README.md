# Simulation of the Relativistic Doppler Shift Effect

This project simulates the relativistic Doppler effect by transforming images according to

\$\$ \lambda' = \frac{\lambda}{\gamma (1 - \beta \cos\theta)} \$\$ 

where \$\lambda'\$ is the transformed wavelength, \$\lambda\$ is the original wavelength, \$\beta = v/c\$ is the velocity as a fraction of the speed of light, \$\theta\$ is the angle of view and \$\gamma\$ is the lorentz factor


## Examples
```python
transform_image(file="example.jpg", beta=-0.15, angle_of_view=np.radians(38))


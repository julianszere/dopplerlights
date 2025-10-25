# Simulation of the Relativistic Doppler Shift Effect on Images

This project was inspired by the well-known joke that at 20% of the speed of light, all red traffic lights would appear green. In fact: 

<img width="1189" height="453" alt="image" src="https://github.com/user-attachments/assets/87bda606-689f-4724-9ab4-b4470c76b9a1" />

---

## Description

An observer moving at relativistic speeds perceives both **color** and **shape** changes due to special relativity. The code simulates this transforming an image according to the **relativistic Doppler effect** and **relativistic aberration** of light.

The wavelength shift follows:

$$
\lambda' = \frac{\lambda}{\gamma (1 - \beta \cos\theta)}
$$

and the aberration warp is: 

$$
\cos\theta = \frac{\cos\theta' + \beta}{1 + \beta \cos\theta'}
$$

where:

- **λ′** – observed (Doppler-shifted) wavelength  
- **λ** – original wavelength  
- **β** $= v / c$ – velocity as a fraction of the speed of light  
- **θ** – angle between the velocity vector and the line of sight  
- **γ** $= 1 / \sqrt{1 - \beta^2}$ – Lorentz factor  

The transformations are computed in **spherical coordinates** $(r, \theta, \phi)$, where the **direction of motion** corresponds to the polar axis. This means that both aberration and Doppler effects depend explicitly on the viewing angle **θ**, with the strongest deformation and color shift occurring along the direction of movement. Approaching sources (β < 0) appear **blue-shifted**, while receding ones (β > 0) appear **red-shifted**.  

---

## Usage Example

```python
transform_image(file="example.jpg", beta=-0.15, angle_of_view=np.radians(38))

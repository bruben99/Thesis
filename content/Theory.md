# Theory
To retrieve the surface of a freeform lens, theory is needed to understand the behavior of how light propagates and interacts with objects. As well as a way to quantify the amount of light hitting a specific object.

## Radiance/Irradiance

First to quantify an amount of light hitting a specific object we Radiance or Irradiance is used. These are the
[//]: # (pipo)

## Ray-Tracing

The behavior of the propagation of light and interaction with free form lenses is best represented by the Maxwell's equations which describe the light as Waves [source]. However in the scope of this thesis, the interaction objects and propagating distances are much bigger in size than the wavelength of the light. This means that the light can be described by the ray optics model[source]. In ray optics some properties like polarization and diffraction are neglected. This makes the computation and modeling of ray optics way easier than the wave model of light.  This model describes the propagation of light along rays. How the rays are bending is described by the Eikonal equation[source: geometrical optics].

[//]: # (pipo2)

$$
\label{Eikonal}
\frac{d}{ds}\left( n(\vec{r},\lambda)\frac{d\vec{r}}{ds} \right) = \nabla n(\vec{r},\lambda)
$$

In this equation, $ds$ is the infinitesimal arc length of the ray path, $n(\vec{r},\lambda)$ is the index of refraction where $\vec{r}$ is the spatial coordinate and $\lambda$ the wavelength of the light. Thus, the index of refraction is both dependent on the medium the light is going through and the wavelength of the light itself.

In the scope of this project, only homogeneous mediums are considered with a constant refractive index. This means that in the Eikonal equation {numref}`Eikonal`.

```{figure} content\figures\Simple_reflection_refraction model.*
:label: Simple refraction
:width: 70%
:align: center

With a 
```

What is ray Tracing, when is it valid
### Mitsuba
What is Mitsuba? explain forward/backward ray tracing


### Differential Ray Tracing
What is differential ray tracing?
What advantage does it have in this case


## Surface-modeling
Describe (TH)Bsplines,
 
How do they work?
Figure of 1d basis functions to create any line

Why would you use them compared to other methods?

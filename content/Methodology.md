# Methodology

## Experimental Part
### Setup

This section will go over the whole experimental setup used to get experimental data. First each section will discuss each 'item' used for the setup. The general setup can be seen in figure {numref}`setup`. 


```{figure}
:label: Setup
:width: 70%
:align: center

This is the setup.
```

#### Robot Arm

The Robot arm can be seen in figure {numref}`Robotarm`. This robot arm is a model???[ref]. This arm has 6 rotational joints to make sure the end point of the arm can be rotated in all 6 degrees of freedom in its working space. The Arm is connected to an PC in the lab where it can be controlled with Python[ref]. The Arm itself has open-source code [ref] where each individual joint can be controlled with 1 degree angles. Also, it is made very easy to set up a Tool center point(TCP), when this is defined it is easy to make relative changes in position and rotation on this point, this is way easier than to define the rotations for each joint separately 
```{figure} 
:label: Robotarm
:width: 70%
:align: center

This is the robot arm used in this thesis.
```

#### LED-Panel
```{figure} 
:label: LED-Panel
:width: 70%
:align: center

This is the LED-panel used in this thesis.
```

```{figure} 
:label: closup LED
:width: 70%
:align: center

This is the LED-panel used as source in this thesis.
```

The LED-panel is connected to a mount on the end of the robot arm. The LED-panel is an Adafruit neopixel 8x8, This panel has 64 LEDs which can be controlled with the PC in the lab where it can be controlled using python[ref]. In {numref}'closup LED' it can be seen that the the LED consists of 4 areas which each scatter a different color of light namely white, red, green and blue. These colors can each individually be controlled with 8-bit input in intensity.

#### Camera
```{figure} 
:label: Camera
:width: 70%
:align: center

This is the Camera used in this thesis.
```
This camera is the exo????? camera[ref] specs:
-mono
-resolution
-
```{figure} 
:label: Imaging Lens
:width: 70%
:align: center

This is the imaging Lens used in this thesis.
```
This imaging lens is used to capture data either on a screen or looking directly at the source.
-f number
-fov
-tunables
Imaging Lens
#### Screen
```{figure} 
:label: Screen
:width: 70%
:align: center

This is the screen used in this thesis.
```
This screen makes sure it can scatter incoming incident light. This scattered light can then be captured by the camera. It also needs to not be transparent otherwise the camera can capture images through it.  
#### Samples
```{figure} 
:label: Sample Convex Lens
:width: 70%
:align: center

This is the convex lens used in this thesis.
```
```{figure} 
:label: Sample freeform
:width: 70%
:align: center

This is the freeform used in this thesis.
```

### Calibration
Now that every 'item' is discussed some calibration is needed in order to do successful ray tracing. Each calibration is discussed below 
#### source
The source has 8 bit options in intensity per color. It is not known yet how these intensities profiles relate to each other. The intensity is needed for the measuring of the camera where this intensity can be related to the strongness of the source in the programming of Mitsuba.

#### Camera intrinsics/Position
Each Camera has certain specs namely principle points, distortion coefficients and focal lengths that are known by the manufacturer of the camera and imaging lens. However, combining these two give of course new parameters that are needed to be measured. These have to be known for the data measured because these intrinsic parameters distort images captured by the camera and imaging lens. With these known raw data can be edited to make sure they represent the reality of the measurement. Also the cameras position is needed to perform raytracing. without this rays will be traced to the wrong position and lens surfaces will be optimised for the wrong images because their position is wrong.

### Measurements (change titel)
With the calibration done now the real measurements can start. As discussed before there are 2 different measurements where

#### Camera
Image of Setup
Different positons of source(how many measurements)

##### Flat source etc

#### Screen
Image of setup
Different positons of source(how many measurements)

##### Flat source etc

## Raytracing

### Mitsuba Scene
How to create the scene

#### Source
Image of source

#### Camera
Camera function mitsuba

#### Screen
irradiance sensor(Bachelor student)
#### Lens Surface
How to define surfaces in Mitsuba

### Optimization

#### Single measuremtn optimization
diagram (illustrator, inkscape), check link in Teams optics Group
#### multiple measuremnts optimization
diagram 
#### Compare/## Validation of Modeling


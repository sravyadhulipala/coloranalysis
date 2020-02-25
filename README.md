# **coloranalysis**
coloranalysis is a python package for calculating the percentage of area covered by one or more colors in an image.

### **Prerequisites**
numpy, opencv and matplotlib are required to execute coloranalysis, you can download them using the following commands:
```
pip install numpy
pip install opencv-python
pip install matplotlib
```

### **Installing**
You can either clone or download this repository, or use this command:
```
pip install coloranalysis
```

### **Usage**
Let us consider this image of a rainbow. 

<img src=https://github.com/sravyadhulipala/coloranalysis/blob/master/coloranalysis/IPTestRainbow.jpg width="400" height="200">

To know the area covered by red color, or the area covered by multiple colors in the image, we should get the HEX codes using a [colorpicker.](https://imagecolorpicker.com/)

Import colorArea, the class that calculates the area of the colors we want, as follows. 
```
from coloranalysis.colors import colorAreas
```
**colorAreas takes no arguments.**
The percentage of area is given by the method getArea, of class colorAreas.
**getArea()** takes three arguments: hexColours (yes, colour with a 'u'), path and diff.
- **hexColours**: A list of strings representing the HEX codes.
- 

See [this notebook]() for an example.

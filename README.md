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

See [this notebook](https://github.com/sravyadhulipala/coloranalysis/blob/master/example/colorAreasExample.ipynb) for an example program on how to use this package. However, reading this document entirely is recommended.

Let us consider this image of a rainbow. 

<img src=https://github.com/sravyadhulipala/coloranalysis/blob/master/example/IPTestRainbow.jpg width="400" height="200">

To know the area covered by red color, or the area covered by multiple colors in the image, we should get the HEX codes using a [colorpicker.](https://imagecolorpicker.com/)

In the above image, HEX codes of all colors are: ["#FE0000", "#FD6400", "#FFFF02", "#008101", "#0000FE", "#4B0081", "#BC31FD"]

Import colorArea, the class that calculates the area of the colors we want, as follows. 
```
from coloranalysis.colors import colorAreas
```
*colorAreas takes no arguments.*

**getArea()** 

The percentage of area is given by the method getArea, of class colorAreas.

*arguments* hexColours (*yes, colour with a 'u' here, we're Indian*), path and diff.
- **hexColours**: A list of strings representing the HEX codes.
- **path**: A string specifying the path of the image.
- **diff**: An integer to determine the lower and upper boundaries of the given colors, in the HSV color space.

*returns* a list of the percentages of area covered by the given colors.

For a digital image as above, the recommended *diff* value is 10. While the recommended *diff* value for images of real-life objects is 30-50. 
For more information on HSV color space, [see this.](https://www.lifewire.com/what-is-hsv-in-design-1078068)

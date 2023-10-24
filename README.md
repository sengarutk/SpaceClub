
# Space Data and its Interpretation

This project deals with data coming from the space through our satellites and how to convert it into pictorial representation including plots and images. 


## Authors

- Utkarsh Sengar 
- Aditya Prabhakar 
- Richa Rajashekhar 
- Shreya S Bhat 


## Acknowledgements

 - [Getting started with FITS file ](https://youtu.be/_DzSIeruotQ?si=UmdYB1thidz49Dkr)
 - [FITS file handling](https://docs.astropy.org/en/v5.0.5/io/fits/index.html#opening-a-fits-file)


## Thought process through the entire journey

This project was accomplished by the collective effort and division of roles in the project.

We have gathered information and  enhanced our learning on the handling and usage of fits file from the documents shared to us and through youtube videos.

We split the task into 4 units with each person handling one unit.

Lightcurve image-Aditya
Lightcurve graph-Shreya
Bonus_image-Richa
Bonus_image graph-Utkarsh

Through this process every member has understood the working of the entire process and have collectively achieved this task.




## Documentation

For interpreting space data, we used Python and its libraries to convert the incoming data into images and scatterplots. 

Modules used: 

- astropy.io: It provides a wide range of functionality and tools for working with astronomical data, performing common calculations and operations used in astronomy, and simplifying the handling of data related to astrophysical observations. 

    But for this project, we only used its ability to read FITS files, which is a common file type in astronomical data. 

- matplotlib: It is a popular and powerful 2D plotting library in Python. It allows you to create a wide variety of high-quality static, animated, or interactive plots and charts for data visualization

    For this project, we used pyplot(), scatter() and plot() functions to plot the data given in the FITS files.

- numpy:  It provides support for working with large, multi-dimensional arrays and matrices of numerical data, along with a vast collection of mathematical functions to operate on these arrays.

    We used where() function to access data according to the condition given in the FITS file and to plot the scatterplot for it. 



 
## Usage/Examples

Using astropy 
```python
from astropy.io import fits

f_file = fits.open('filename.fits') 
f_file.info()
```

Using matplotlib
```python 
import matplotlib.pyplot as plt 
plt.figure() #Generates a figure 
plt.imshow(imdata, origin = 'lower') #Displays the image 
plt.colorbar() #Adds a gradiented colorbar to the image 
plt.show() #Displays the image as a graph with colorbar
```

Using numpy 
```python
import numpy as np 
wp = np.where(condition) #checks if the given condition is true 
plt.plot(x[wp],y[wp]) #plots the point where the given argument satisifes
plt.show()  #displays the graph 
```




## Screenshots
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_26_44](https://github.com/sengarutk/SpaceClub/assets/148872020/2ebb1b54-c628-42ba-87fc-df62e1a5de7e)
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_26_53](https://github.com/sengarutk/SpaceClub/assets/148872020/5c9f2a2b-a009-4a10-8163-53b32c2b2ab6)
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_27_08](https://github.com/sengarutk/SpaceClub/assets/148872020/b9898950-c2df-4cc8-960c-70c944ce99a2)
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_27_13](https://github.com/sengarutk/SpaceClub/assets/148872020/38ef7ad6-a85c-440b-a624-d3f91b216a15)









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


![file ipynb - Space club - Visual Studio Code 10_23_2023 16_26_44](https://github.com/sengarutk/SpaceClub/assets/148872020/1c7e6a0e-aafe-4ba1-ae75-c049816ce63a)
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_26_53](https://github.com/sengarutk/SpaceClub/assets/148872020/ddbdcaee-f0b4-463c-8e1c-6edbf3623951)
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_27_08](https://github.com/sengarutk/SpaceClub/assets/148872020/56c22bba-e0a0-45bf-9b53-a2ea5858b18a)
![file ipynb - Space club - Visual Studio Code 10_23_2023 16_27_13](https://github.com/sengarutk/SpaceClub/assets/148872020/98edc962-7c05-4675-8be8-00575090f3c2)



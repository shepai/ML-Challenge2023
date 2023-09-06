# ML-Challenge 2023
## Task
Your task is to classify sensor data to determine whether the movement is part of walking or driving. The data set has been prepared with columns representing time step, action (1 for walking and 4 for driving), and then the acceleration in the x, y and z. This data is a subset of the data from <a href="https://physionet.org/content/accelerometry-walk-climb-drive/1.0.0/#files">this dataset</a>. 

## Downloading the data
You can simply download the csv file or clone this repository. Once you have the csv file local you can open and view it with pandas:
```
import pandas as pd

df=pd.read_csv("path/to/file/movementSensorData.csv")
print(df)
```
You should get something like this:
```
       activity  time_s   lw_x   lw_y   lw_z
66077         1  660.78  0.066 -1.270 -0.020
66078         1  660.79  0.082 -1.281 -0.063
...         ...     ...    ...    ...    ...
```


## Rules
You must be an undergraduate or master's student. 



# Bibliography
Karas, M., Urbanek, J., Crainiceanu, C., Harezlak, J., & Fadel, W. (2021). Labelled raw accelerometry data captured during walking, stair climbing and driving (version 1.0.0). PhysioNet. https://doi.org/10.13026/51h0-a262.

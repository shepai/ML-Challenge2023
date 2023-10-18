import matplotlib.pyplot as plt
import pandas as pd
import numpy as np

def visualiser(df):
	print(df.keys())
	x=df.loc[df['activity'] == 1, 'lw_x']
	y=df.loc[df['activity'] == 4, 'lw_x']
	plt.plot(x,label="Walking x-axis")
	plt.plot(y,label="Driving x-axis")
	plt.legend(loc="upper right")
	plt.xlabel("Time step")
	plt.ylabel("Value")
	plt.show()

	x=df.loc[df['activity'] == 1, 'lw_y']
	y=df.loc[df['activity'] == 4, 'lw_y']
	plt.plot(x,label="Walking y-axis")
	plt.plot(y,label="Driving y-axis")
	plt.legend(loc="upper right")
	plt.xlabel("Time step")
	plt.ylabel("Value")
	plt.show()

	x=df.loc[df['activity'] == 1, 'lw_z']
	y=df.loc[df['activity'] == 4, 'lw_z']
	plt.plot(x,label="Walking z-axis")
	plt.plot(y,label="Driving z-axis")
	plt.legend(loc="upper right")
	plt.xlabel("Time step")
	plt.ylabel("Value")
	plt.show()
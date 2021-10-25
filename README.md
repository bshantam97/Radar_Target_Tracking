## Author : Shantam Bajpai
# Radar_Target_Tracking

## Description
This is the final project of the RADAR course , which is part of the sensor fusion nanodegree offered by Udacity. The layout of the project was as follows.

<img src="Final_project_workflow.png" width="620" height="350" />

Given the RADAR parameters we had to configure the FMCW (Frequency modulated continuous waveform) waveform based on the system parameters. After the completetion of this step compute the beat signal which is nothing but the mixing of the Recieved and the transmit signal. On this beat signal compute the Fast Fourier Transform across the range dimension and compute the single sided spectrum that will give a peak at a certain range based on our initial setting of the vehicle range. After Range FFT computation I performed the 2D CFAR (Constant False Alarm Rate) for noise thresholding of the output 2D FFT which gave me the target response with the (X,Y,Z) axes denoting the range velocity and signal strength.

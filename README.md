# gesture_recognition


# Notes & Observations:
1)	Simple models created with multiple layers and run in local CPU environment
2)	Optimal values:
	a.	Batch size = 16
	b.	Image selection – every 1 image of 30
	c.	Learning Rate – 0.0004
3)	LTSM learns slow followed by GRU and CNNs are fast but closely comparable to GRU models
4)	CNN models look accurate as well with fewer training epochs needed 


# Future Experiments:
1)	Reduced or increased middle layers
2)	Bias parameter is not added, but can be included 
3)	Same padding considered to make the experiments comparable, however in further experiments we can change this parameter
4)	Timing calculation of runs of different models, added in 3rd experiment but did not include as it was missed on early experiments
5)	Had tried with 64*64 resized images, but accuracy was lesser, however since it was not saved, mentioned under further experiments.


# Metrics & Experiments
Refer to https://github.com/anjithan/gesture_recognition/blob/master/writeup_gesture_recognintion_case_study.doc


# Libraries
Refer to jupyter notebook which has the pip list at the end


# Author
@anjithan or jithan.an@gmail.com


# Acknowledgements
Googled to look at other similar experiments
Starter code was provided


# gesture_recognition
Metrics/Experiments	Experiment 1	Experiment 2	Experiment 3
Batch Size	16	16	32
Image selection (of 30)	every 2nd	every 1	every 1
Image resize value	128*128	128*128	128*128
num epochs	50	50	30
			
CNN Model - Training accuracy	0.8902	0.8363	0.8795
CNN Model - Validation accuracy	0.7857	0.8304	0.5625
Learning Rate - suited	0.0004	0.0004	0.002
Suited LR found at epoch	41	38	23
CNN Model - Training accuracy at LR 	0.8628	0.881	0.8423
CNN Model - Validation accuracy at LR 	0.8214	0.875	0.7734
Params	Total params: 1,146,565	Total params: 1,146,565	Total params: 1,146,565
	Trainable params: 1,145,701	Trainable params: 1,145,701	Trainable params: 1,145,701
	Non-trainable params: 864	Non-trainable params: 864	Non-trainable params: 864
			
GRU Model - Training accuracy	0.5503	0.8676	0.8765
GRU Model - Validation accuracy	0.6071	0.7143	0.5547
Learning Rate - suited	0.0004	0.0004	1.60E-05
Suited LR found at epoch	50	22	30
GRU Model - Training accuracy at LR 	0.5503	0.8705	0.8765
GRU Model - Validation accuracy at LR 	0.6071	0.7411	0.5547
Params	Total params: 3,302,629	Total params: 3,302,629	Total params: 3,302,629
	Trainable params: 3,302,149	Trainable params: 3,302,149	Trainable params: 3,302,149
	Non-trainable params: 480	Non-trainable params: 480	Non-trainable params: 480
			
LTSM Model - Training accuracy	0.8293	0.8824	0.8646
LTSM Model - Validation accuracy	0.625	0.6964	0.5938
Learning Rate - suited	0.0004	0.0004	1.60E-05
Suited LR found at epoch	47	19	30
LTSM Model - Training accuracy at LR 	0.8201	0.8854	0.8646
LTSM Model - Validation accuracy at LR 	0.625	0.7054	0.5938
Params	Total params: 4,367,333	Total params: 4,367,333	Total params: 4,367,333
	Trainable params: 4,366,853	Trainable params: 4,366,853	Trainable params: 4,366,853
	Non-trainable params: 480	Non-trainable params: 480	Non-trainable params: 480

Notes & Observations:
1)	Simple models created with multiple layers and run in local CPU environment
2)	Optimal values:
a.	Batch size = 16
b.	Image selection – every 1 image of 30
c.	Learning Rate – 0.0004
3)	LTSM learns slow followed by GRU and CNNs are fast but closely comparable to GRU models
4)	CNN models look accurate as well with fewer training epochs needed 



Future Experiments:
1)	Reduced or increased middle layers
2)	Bias parameter is not added, but can be included 
3)	Same padding considered to make the experiments comparable, however in further experiments we can change this parameter
4)	Timing calculation of runs of different models, added in 3rd experiment but did not include as it was missed on early experiments
5)	Had tried with 64*64 resized images, but accuracy was lesser, however since it was not saved, mentioned under further experiments.

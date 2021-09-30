Noisy data are created adding an additive white gaussian noise to the data obtained by simulation.

the reference batch for data is made of 20 datasets (speeddata1 to speeddata20) corresponding to 20 different values of backlash.

noisy signals are created adding the noise-only signal to original noise-free signals.
noise-only signal= Noise_Amplitude*(rand(length(Speeddata),1)-0.5) 
->actual noise amplitude will be Noise_Amplitude=0.5

Two differennt level of noise are considered: 
	Low level - Noise amplitude from A_min=0.2/2 to A_max=0.5/2 


	High level - Noise amplitude from A_min=1.5*(0.2/2) to A_max=1.5(0.5/2) 


For each batch of noisy signals many oucames can be evaluated.
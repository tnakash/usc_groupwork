# usc_groupwork
## General
DNN based predictor of 2D Lid-driven cavity flow by inputting Reynolds number.  
For now it can predict distribution of either u or w (33*33).  
  
Used Keras module, referring Zhou and Ooka (2020).  
Used csv dataset kindly prepared by Sakamoto san from NMRI.  
Devide Training and Test dataset into 9:1. Epoch number is set to be 50.  

## Note
Set input directory which all the input files are in, and output directory which the figure comparing DNN and CFD of test data.  
Model hyper-parameters setting is yet to be done (hidden layers, num of neurons, activation function, optimizer and learinging rate...), So please GIVE IT A TRY!

## Author
Takuya Nakashima  
University of Tokyo

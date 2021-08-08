# usc_groupwork
## General
DNN based predictor of 2D Lid-driven cavity flow by inputting Reynolds number.  
It can predict distribution of ~~either u or w (33*33)~~ both u and w (33*33).  
Used csv dataset kindly prepared by Sakamoto san from NMRI. (("velocity_[1-100].csv")  
Devided Training and Test dataset into 9:1.  

### USC_group4.ipynb (1D DNN)
Used Keras module (Sequential API, but might be readable using Functional API).  
Set hyperparameters referring Zhou and Ooka (2020). Used MSE for loss function.  
Set epoch number to be 50 and confirmed to be converged.  

### USC_group4_CNN.ipynb (Deep CNN)
Used Keras module (Sequential API) and created Decoder, referring the following pages.
https://qiita.com/koshian2/items/f4917b1e6c944674fb80
Set hyperparameters as follows; Adam for Optimizer, MSE for Loss Function.
Used 16-32 kernels (3*3) and Upsampling (1*1→2*2).  
Use batch normalization for all layers.  
https://www.scsk.jp/product/oss/tec_guide/tensorflow_keras/1_tensorflow_keras2_2.html
Set epoch number to be 50 and confirmed to be converged.

## Note
Set input directory which all the input files are in, and output directory which the figure comparing DNN and CFD of test data.  
Model hyper-parameters tuning is yet to be done. PLEASE RESET AND TRY!

## Author
Takuya Nakashima  
University of Tokyo

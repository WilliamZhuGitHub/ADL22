# ADL22

# 1. Introduction
  1. I added more dense layers and made it deeper. It beat the goal of linear regression’s 24.29 MSE.  
  2. Increasing the amount of neurons will make the NN more overfitted towards the training data.

# 2. Intro to convolution operations: padding
  1.	A response layer is the filter after using the convolution.  
  2.	32 means 32 different filters. Each filter is 26x26 
  3.	The response shape will be a 4x4 and have 16 responses
  4.	32x32 
  5.	Valid means there’s no padding. Same padding is when padding is automatically added so that output size is the same as input size. Given a 6x6 input and 3x3 filter       the valid response shape would be 4x4 and the same response would be 6x6. 
# 3. Convolution parameters: stride and pooling
  1.	Max pooling is used to down sample to reduce weights
  2.	The resulting size is 3x3 

# 4. ConvNet Architectures, layers
  1.	I: Input Volume, F: Filter, S: Stride, P: Zero Padding, O: Output Size
  2.	(100-2+(2*0)/1)+1 =  output size = 98
  3.	2*2*24 = 96 weights
  4.	((S-1)*I – S+F) /2
  5.	
# 5. Practical Patterns
  1.	ImageDataGenerator is used to modify images while the model is still training. This can be useful in the case of overfitting. 
  2.	Using small kernel sizes is better because larger kernels take more time to train. 4(2,2) is 16 weights whereas 8x8 is 64 weights. 
 



	



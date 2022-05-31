# ADL22

# 1. Introduction
  1. I added more dense layers and made it deeper. It beat the goal of linear regression’s 24.29 MSE.  

![image](https://user-images.githubusercontent.com/56366459/171251747-14781a96-af83-4ac3-a9e8-d080e85d0929.png)

  3. Increasing the amount of neurons will make the NN more overfitted towards the training data.

# 2. Intro to convolution operations: padding
  1.	A response layer is the filter after using the convolution.  
  2.	Given (26,26,32), the 32 means 32 different filters. Each filter is 26x26.
  3.	The response shape will be a 4x4 and have 16 responses
  4.	The response shape is 32x32.
  5.	Valid means there’s no padding. Same padding is when padding is automatically added so that output size is the same as input size. Given a 6x6 input and 3x3           filter the valid response shape would be 4x4 and the same response would be 6x6. 
# 3. Convolution parameters: stride and pooling
  1.	Max pooling is used to down sample to reduce weights.
  2.	The resulting size is 3x3.

# 4. ConvNet Architectures, layers
  1.	I: Input Volume (Size of the input),  F: Filter (Size of the kernel), S: Stride (Distance between successive windows), P: Zero Padding (Padding added to the 	     edges), O: Output Size (Size of the output).
  2.	(100-2+(2*0)/1)+1 =  The output size = 98
  3.	2x2x24 = 96 weights
  4.	To get the same input and output size p has to be equal to p = ((S-1)*I – S+F) /2
 
# 5. Practical Patterns
  1.	ImageDataGenerator is used to modify images while the model is still training. This can be useful in the case of overfitting. 
  2.	Using small kernel sizes is better because larger kernels take more time to train. 4(2,2) is 16 weights whereas 8x8 is 64 weights. 
 



	



1.Download and import the Tensorflow and other required libraries
2.Import the 'CIFAR10'test and train datasetsusing the Kerasandthe train  and  test  labels. 
Also,  scale  the  datasets  by  dividing  with  a common number
3.Define  the  class  names  as -['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
for class of images
4.Define  a  sequential  convolutional  base  using  common  patterns Conv2D and MaxPooling2D layers 
(use 'relu'(Rectified Linear Unit)activation function)Note:As   input,   a   CNN   takes   tensors   of   shape   (image_height
image_width, color_channels), ignoring the batch size. If you are new to  these  dimensions,  color_channels  refers  to  
(R,  G,  B).  In  this example, you will configure your CNN to process inputs of shape (32, 32, 3), which is the format of CIFAR images. Wecan do this by passing the argument input_shape to your first layer.
5.Feed the final output tensor from the convolutional base into one or more Dense layers to perform classification.
Note:Dense  layers  take  vectors  as  input  (1D),  while  the  current output is a 3D tensor. 
First, We will flatten (or unroll) the 3D output to  1D,  then  add  one  or  more  Dense  layers  on  top.  
CIFAR  has  ten output classes, so we use a Dense final layer with ten outputs.
6.Compile and train the model
7.Calculate and print the test accuracy of the model                                                                                                             

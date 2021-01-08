# Project2
## LeNet and Keras
  In this project,I choose LeNet and Keras.Each one has parameters modified, and each one has three methods  
  
1.LeNet  
    LeNet-Lab-solution.ipynb is similiar to the example in the lession.The main thing is to check the environment of tenserflow and check what packages is missing.Because the need of a low version.And the example runs with a little warning.But I finally figure out the answers and accuracy.  
    LetNet-Lab-convolution.ipynb adds a layer of convolution3.I make a comments in the code.Input=5*5*16 become Input=3*3*32.And make the dimensions small.I want to conpare the results with the examples in class.Alos,in the fully connected.I change the output to see what happens if I change the parameters.Finally,I use "fc2 = tf.nn.dropout(fc2, 0.5)" to make a dropout to prevent overflow.  
    LetNet-Lab-Conv&Stride&FC.ipynb changes the stride and adds a layer of fully connected what I have made a comments in the code.In the step of Conv2,I modify the steide from one to two to see what happen.And the results make a different chance.Also,I adds a layer of fully connected make Input=64 to Output=30.Besides,I make a dropout in the end.  
    The resluts of accuracy is listing as following.The results is solution,concolution,Conv&Stride&Fc.

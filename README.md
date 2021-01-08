# Project2
## LeNet and Keras
In this project,I choose LeNet and Keras.Each one has parameters modified, and each one has three methods  
  
1.LeNet  
LeNet-Lab-solution.ipynb is similiar to the example in the lession.The main thing is to check the environment of tenserflow and check what packages is missing.Because the need of a low version.And the example runs with a little warning.But I finally figure out the answers and accuracy.  
    
LetNet-Lab-convolution.ipynb adds a layer of convolution3.I make a comments in the code.Input=5*5*16 become Input=3*3*32.And make the dimensions small.I want to conpare the results with the examples in class.Alos,in the fully connected.I change the output to see what happens if I change the parameters.Finally,I use "fc2 = tf.nn.dropout(fc2, 0.5)" to make a dropout to prevent overflow.  
    
LetNet-Lab-Conv&Stride&FC.ipynb changes the stride and adds a layer of fully connected what I have made a comments in the code.In the step of Conv2,I modify the steide from one to two to see what happen.And the results make a different chance.Also,I adds a layer of fully connected make Input=64 to Output=30.Besides,I make a dropout in the end.  
    
The resluts of accuracy is listing as following.The results is solution,concolution,Conv&Stride&Fc.  
<div align=center><img src="https://github.com/zzy-98012/Project2/blob/main/iamge/solution.PNG" height="200" width="100"/></div>
<div align=center><img src="https://github.com/zzy-98012/Project2/blob/main/iamge/solution.PNG" height="200" width="100"/></div>
<div align=center><img src="https://github.com/zzy-98012/Project2/blob/main/iamge/solution.PNG" height="200" width="100"/></div>  

We can see that the accuracy of the first and second methods is similar.But the accuracy of the third method drops rapidly.I guess it's because I changed the stride.Becacuse the 'padding=VALID'.Maybe some data is discarded during the whole operation.There may be other reasons because I don't understand the whole algorithm as well  

2.Keras  

Keras1 changes the second of ConV2D.I change with the code 'model.add(Conv2D(32, (3, 3), input_shape=(15, 15, 16)))'.And I add a Dropout with the parameter of 0.5.Also I change the Dense(100) into Dense(512) which is different of the examples.But I think the change of Dense is not important.  

Keras2 is similar to the Keras1.The Keras2 is without the dropout.I also add a ConV2D and change the Dense.  

Keras3 is the example in the book.There are no changes.It have no dropout and only once ConV.Of course,the result is the lowest.  

The resluts of accuracy is listing as following.The results is Keras1,Keras2,Keras3.  

# Final_Exam_20216017

- > This repo was created to submit the final assignments for the open source sw class.

#1. method : I made a model to classify images using LogisticRegression.

#2. insert code :

...python
log_reg = sklearn.linear_model.LogisticRegression(max_iter = 450, C = 1050, random_state=1)
log_reg.fit(X_train,y_train)
y_pred = log_reg.predict(X_test)
...

explantion : I created a model called log_reg ( = short for LogisticRegression) using the sklearn package. And, trained the model using X_train and y_train. 

#3. Hyper parameter of the funcion: 
I use C and the max_iter parameter to increase the accuracy.

At first, the max_iter was adjusted by raising and lowering it from 500 to 1000, and the change in accuracy was observed accordingly. After adjusting max_iter to about 500~1000, I adjusted the C parameter. The observed accuracy while adjusting the C parameter was between 72 and 98, and the approximate range of C corresponding to 98, which was the highest accuracy, was found. I had an accuracy of 98 when value of C was near 1020 and 1050, and strangely, when it was 1035, the median value, the accuracy was reduced by one. Finally, the C value was adjusted to 1050.

To further increase the accuracy, I observed the change in accuracy by changing the max_iter value while keeping the C value fixed. If max_iter was lowered below 400, an error occurred and it could not be lowered further, and the accuracy did not change no matter how much it increased above 400. Finally, the max_iter value is set to 450, and the final accuracy is 98%.



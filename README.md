	This is my model for cs50 ai project 5 traffic.
		What did you try?
The model is saved as 'gtsrb_model.h5'. It consists of the following:
	1. Two convolution layers
	2. One Max pooling layer
	3. Two dropout layers
	4. A flatten layer
	5. Two dense layers
When the model was run, it got an accuracy = 98.10 % and loss = 7.53 %.
After doing a couple of experiments like,
	(i) When the number of convolutional layers was changed from two to three and the number of max-pooling layers was changed from
one to two, accuracy = 96.27 % and loss = 13.44 %
	(ii) When the number of convolutional layers was changed from two to three and the size of convolutional layer with 128 filters
was changed to 64 filters, accuracy = 97.50 % and loss = 9.21 %
	(iii) When the max-pooling layer's size was changed from (3, 3) to (5, 5), accuracy = 93.72 % and loss = 21.8%
	(iv) When the number of Dense layers was changed from two to threee accuracy = 94.11 % and loss = 21.36 %
	(v) When number of dropouts changed from two [0.5 and 0.5] to three [0.5, 0.75, 0.25], accuracy = 89.0 % and loss = 35.94 %

		What worked well....?
(i) and (ii) gave results which were good, while (iii) and (iv) gave results which were close
		
		What didn't work well.....?
(v) gave results which were not much close to the actual one.

		What did you notice?
In (i), adding convolutional layer , created overfitting in the model.
In (ii), When the number of convolutional increased with the decrease in number of neurons in other layer, a slight decrease was noticed.
In (iii), greater Max-pooling layer created reduction in the precision of image, which reduced accuracy
In (iv) the increase in the dense layers, made over-reliance on the data.
In (v), When the dropout was made too much, there only little data was able to be retreived from the image and hence accuracy declined.
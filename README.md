# Images-Classification---Fashion-Mnist-Dataset
This project examines the performance of a variety of machine learning methods on the fashion mnist dataset.
Image classification is performed using k nearest neighbors , support vector machines , neural networks with two hidden layers and bayes methods.
Of course the performance varies from method to method and depends on the parameters given by the user as input.

The first class of the program is responsible for preprocessing the images in the dataset. 
The function def normalization , normalizes the pixel values of each image , as it converts them from the range 0-255 , to the range 0-1(float). 
The next function in the class , dimensions_reduce , reduces the dimensions of the images , depending on the input received from the user 
(For example, if the user gives 70 as input , then after processing , 70% of the size of the original images remains). 
These procedures lead to the reduction of the data volume , resulting in the program making faster predictions.

In the next class all the work for categorization is performed.
In fact with the help of the scikit learn library , each function is built in a similar way. 
Training is done with the train data and then the predictions are made on the test data. 
The visualization function is responsible for visualizing the images and displaying the metrics of each method. 
The visualization and display of the metrics is done in two ways. One is for knn, svm and bayes methods and the other is for neural_network_2hlayers.
In the first case a table with several metrics(accuracy , precision, recall, f1-score) is displayed accompanied by a sample of 10 images ,
where the actual label is indicated and next to it the prediction.
In the second case concerning the method with neural networks , due to the softmax activation function in the output layer,
the probabilities of each object belonging to each category are printed.

The conclusion is that the best methods are Support Vector Machines ,Neural Networks, Knn. 
Bayes method has the lowest performance and it depends on the dimensions of the images given as input(The smaller the dimensions , the better the accuracy).


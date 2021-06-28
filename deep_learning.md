### Deep Learning

Q. What is a 'Bottleneck' layer?       
A. A bottleneck is an informal term often used for the layer just before the final output layer that actually does the classification.

* Different types of accuracy metrics:    
  * Training Accuracy   
    * The training accuracy shows the percentage of the images used in the current training batch that were labeled with the correct class.
Validation accuracy is the precision (percentage of correctly-labelled images) on a randomly-selected group of images from a different set.
Cross entropy is a loss function that gives a glimpse into how well the learning process is progressing (lower numbers are better here).

A true measure of the performance of the network is to measure its performance on a data set that is not in the training data. This performance is measured using the validation accuracy. If the training accuracy is high but the validation accuracy remains low, that means the network is overfitting, and the network is memorizing particular features in the training images that don't help it classify images more generally.

The training's objective is to make the cross entropy as small as possible, so you can tell if the learning is working by keeping an eye on whether the loss keeps trending downwards, ignoring the short-term noise.

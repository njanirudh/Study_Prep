### Deep Learning

#### Architecture

<details>
  <summary> Difference between regularization and normalization? </summary> 
 
 [(src)](https://stackoverflow.com/questions/47014365/what-is-the-difference-between-normalisation-and-regularisation-in-machine-learn#:~:text=1%20Answer&text=Normalisation%20adjusts%20the%20data%3B%20regularisation,as%20standard%20deviation%20and%20mean.)
  1. Regularization
    * Regularisation adjusts the prediction function.
  1. Normalization
    * Normalisation adjusts the data to have same scale.
</details>

<details>
  <summary> Different types of regularization techniques in deep learning? </summary> 
 
 [(src)]()
  * Dropout
  * Reduce model size
  * Increase dataset (Data augmentation)
  * Early stopping
</details>


<details>
  <summary> Different types of normalization techniques? </summary> 
 
 [(src)]()
  * 
  * 
</details>

<details>
  <summary> Batch Norm </summary> 
 
 [(src)]()

</details>

<details>
  <summary> Object detection architectures </summary> 
 
 [(src)]()

</details>

<details>
  <summary> Forward pass and Backward pass </summary> 
 
 [(src)]()

</details>

<details>
  <summary> 'Bottleneck' layer </summary> 
 
 [(src)]()
 A bottleneck is an informal term often used for the layer just before the final output layer that actually does the classification.
  
</details>

<details>
  <summary> Model bias and variance ?</summary> 
 
 [(src)]()
</details>

<details>
  <summary> Model bias vs Data bias ?</summary> 
 
 [(src)]()
</details>


#### Training

<details>
  <summary> Overfitting and Underfitting ?</summary> 
 
 [(src)]()
</details>

#### Maths

<details>
  <summary> Backpropogation </summary> 
 
 [(src)]()

</details>

<details>
  <summary> Gradient descent, Mini-batch GD, Stochastic GD ? </summary> 
 
 [(src)](https://datascience.stackexchange.com/questions/36450/what-is-the-difference-between-gradient-descent-and-stochastic-gradient-descent)

</details>


<details>
  <summary> What is the stochastic component in Stochastic Gradient Descent ? </summary> 
 
 [(src)](https://datascience.stackexchange.com/questions/36450/what-is-the-difference-between-gradient-descent-and-stochastic-gradient-descent)
</details>

<details>
  <summary> Different types of optimizers ? </summary> 

 [(src)]()
  1. Gradient Descent
  1. Momentum based
  1. Adam (adaptive moment estimation)
</details>


#### Classification Metrics

<details>
  <summary> Why is accuracy a bad metric? </summary> 
 
 [(src)]()
Accuracy gives wrong predictive confidance in an class-imbalanced data set.

</details>

<details>
  <summary> Classification: Precision and Recall </summary> 
 
 [(src)](https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall)
* Precision
  * What proportion of positive identifications was actually correct?
  * Precision = TP/(TP + FP)
 
* Recall
  * What proportion of actual positives was identified correctly?
  * Recall = TP /(TP + FN)
 
</details>

<details>
  <summary> Effect of Threshold on Precision and Recall? </summary> 
 
 [(src)]()
 * Increasing classification threshold.
   * In general, raising the classification threshold reduces false positives, thus raising precision.
 * Decreasing classification threshold.
   * Raising our classification threshold will cause the number of true positives to decrease or stay the same and will cause the number of false negatives to increase or stay the same. Thus, recall will either stay constant or decrease.

</details>


<details>
  <summary> F1 score </summary> 
 
 [(src)]()

</details>

<details>
  <summary> ROC curve (receiver operating characteristic curve)  </summary> 
 
 [(src)](https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc)
ROC curve shows the performance of a classification model at all classification threasholds.
It is a graph between Precision (True Positive Rate) and False Positive Rate (FPR) . 

</details>

<details>
  <summary> Area under the curve of ROC curve </summary> 
 
 [(src)](https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc)


</details>

<details>
  <summary>High Precision or High Recall? </summary> 
 
 [(src)](https://medium.com/analytics-vidhya/precision-recall-tradeoff-for-real-world-use-cases-c6de4fabbcd0)
* High Recall:
  * When you cannot afford to have any false negatives, you prioritize recall.
  * When you cannot afford to miss any detection, you look for high recall
  * Medical test (eg. cancer detection), Not Safe For Work (NSFW) images detection
* High Precision
  * When you cannot afford to have any false positives, you prioritize precision.
  * when you cannot afford to have any incorrect detection you look for high precision. 
  * Recommendation Systems, Predicting a good day based on weather conditions to launch satellite, Criminal death punishment, Email spam detection

</details>

<details>
  <summary>What are Type 1 and Type 2 errors? </summary> 
 
 [(src)](https://en.wikipedia.org/wiki/Precision_and_recall)


</details>




<details>
  <summary> Different types of Accuracy metrics </summary> 
 
 [(src)]()
 
  * Training Accuracy   
    * The training accuracy shows the percentage of the images used in the current training batch that were labeled with the correct class.
Validation accuracy is the precision (percentage of correctly-labelled images) on a randomly-selected group of images from a different set.
Cross entropy is a loss function that gives a glimpse into how well the learning process is progressing (lower numbers are better here).

    * A true measure of the performance of the network is to measure its performance on a data set that is not in the training data. This performance is measured using the validation accuracy. If the training accuracy is high but the validation accuracy remains low, that means the network is overfitting, and the network is memorizing particular features in the training images that don't help it classify images more generally.

    * The training's objective is to make the cross entropy as small as possible, so you can tell if the learning is working by keeping an eye on whether the loss keeps trending downwards, ignoring the short-term noise.

</details>


  



no. of Chris training emails: 4406  

no. of Sara training emails: 4383

***

## Naive Bayes
training time:  2.792 s  
testing time:  0.319 s  
Accuracy of author identification by Naive Bayes classifier is :  0.973265073948  
Prediction time of Naive bayes is less than the training time. 


*** 

## SVM
#### SVM with a linear kernel
training time:  91.523 s  
testing time:  75.428 s  
Accuracy of author identification by SVC classifier is :  0.981226533166

So SVM is much slower to train and predict than Naive Bayes classifier.

#### SVM after reducing the training data size
training time:  0.072 s  
testing time:  3.103 s  
Accuracy of SVC classifier is :  0.925702582774 or 93% (Approx)

#### SVM after changing the kernel to 'rbf'
training time:  0.281 s  
testing time:  1.094 s  
Accuracy of SVC classifier is :  0.892491467577

#### SVM after changing the kernel to 'rbf' and C = 10000 and with full data
training time using rbf kernel (and C = 10000.0) :  140.817 s  
testing time using rbf kernel (and C = 10000.0) :  15.599 s  
Accuracy of SVC classifier after using rbf kernel (and C = 10000.0) is :  0.990898748578 

***

Naive Bayes is great for text--it’s faster and generally gives better performance than an SVM for this particular problem. Of course, there are plenty of other problems where an SVM might work better. Knowing which one to try when you’re tackling a problem for the first time is part of the art and science of machine learning. In addition to picking your algorithm, depending on which one you try, there are parameter tunes to worry about as well, and the possibility of overfitting (especially if you don’t have lots of training data).

Our general suggestion is to try a few different algorithms for each problem.

***
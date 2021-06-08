## Alzheimer's Disease Prediction
- ***Oğuzhan DURSUN*** 

- ***Alperen Toraman*** 

![image](https://user-images.githubusercontent.com/72974967/121230763-53b6b880-c898-11eb-9cb8-f7da5a7aaa1e.png)

In this project, we are trying to accurately diagnose the various stages of Alzheimer's Disease, which is a disease that occurs especially in advanced ages and decreases the quality of life, by using different classification methods through magnetic resonance images.  To accomplish this goal we used methods such as KNN, SVM, Random Forest, DenseNet and VGG16. After evaluating the results of those methods, DenseNet has the most accurate result with 86.91% accuracy.

Alzheimer's is a common type of dementia, a progressive neurological disease that causes brain cells to be destroyed.  In this disease which causes decrease in thought, memory and behavioral functions, symptoms reveal themselves as the age of the patient increases.
Alzheimer's is a disease with no definitive treatment, but with early diagnosis, the progression of the disease and the decline in the patient's quality of life can be slowed down. Early symptoms of Alzheimer's may not be taken seriously and might be associated with old age.  With this project pre-diagnosis of any patient with suspicion of Alzheimer can be done easily and quickly.


Our dataset consists of brain MRIs of patients with suspicion on Alzheimer’s Disease. Those MRIs are classified for train and test sets.  There are four stages of Alzheimer’s Disease in our dataset those are:
*	Moderate Demented
*	Mild Demented
*	Very Mild Demented
*	None Demented

![image](https://user-images.githubusercontent.com/72974967/121230839-6630f200-c898-11eb-816c-6f36a227dfe4.png)
![image](https://user-images.githubusercontent.com/72974967/121230913-75b03b00-c898-11eb-90a7-309c1b904efc.png)
![image](https://user-images.githubusercontent.com/72974967/121230995-8a8cce80-c898-11eb-8321-daf0b0868fb9.png)


In our project, instead of sticking to a single machine learning model, we aimed to achieve the highest success rate by researching various algorithms that are widely used and creating their models. Algorithms such as KNN, Random Forest, SVM, which were our first experiments, achieved lower success in classification than the CNN models we created later. Based on our research and conclusions, we decided that there were many reasons for this situation. Some of these reasons are:
* Although KNN performed well in data sets with high data count, our data set was not as large as desired, and at the same time, the fact that the size of the data set was not provided badly affected the performance of the KNN algorithm in image classification, and our data set consisted of multiple classes also adversely affected the performance of the KNN algorithm.


* Although the Random Forest algorithm copes well with the overfitting problem, it is unfortunately not a successful algorithm for classifying images. The reason for this is that the pixel information transferred to the array by image processing is perceived as too many features to be difficult while being processed by the Random Forest algorithm.


* The SVM algorithm is inherently not suitable for multi-class data. Despite the changes made to work with multiple classes, it could not achieve a noticeable success because its nature was not suitable for it.


CNN algorithms are visibly more successful than these three algorithms. The reasons for this are:

* CNN algorithms are very successful in classifying images because they are designed to distinguish a large number of features (pixels for images) that are homogeneous.

* CNN algorithms can take advantage of this design advantage and find the important features among the features they distinguish without the need for human supervision.


Dataset link: https://www.kaggle.com/tourist55/alzheimers-dataset-4-class-of-images
Youtube link: https://youtu.be/uA5VYqBHwT8

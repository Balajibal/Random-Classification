# RANDOM CLASSIFICATION
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Related Theoritical Concept:
Multiclass Classification
In multi-class classification, the neural network has the same number of output nodes as the number of classes. Each output node belongs to some class and outputs a score for that class. Class is a category for example Predicting animal class from an animal image is an example of multi-class classification, where each animal can belong to only one category.

The number of classifier models depends on the classification technique we are applying to. •One vs. All:- N-class instances then N binary classifier models •One vs. One:- N-class instances then N* (N-1)/2 binary classifier models •The Confusion matrix is easy to derive but complex to understand.

## Algorithm
1.define dataset with centers=3 
2.summarize dataset shape 
3.ummarize observations by class label 
4.summarize first few examples 
5.plot the dataset and color the by class label

## Program:
```
/*
Program to implement random classification.
Developed by   : balaji N
RegisterNumber :  212220230006
*/
```
import matplotlib.pyplot as plt
from sklearn import datasets
x,y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)

fig = plt.figure(figsize = (10,8))
plt.plot(x[:, 0][y==0],x[:, 1][y==0],'bs')
plt.plot(x[:, 0][y==1],x[:, 1][y==1],'g^')
plt.xlabel("feature 1")
plt.ylabel("feature 2")
plt.title("Random classifiction data with 2 classes")

## Output:
![Screenshot (57)](https://user-images.githubusercontent.com/75234946/162910739-ae26bb7a-4c5e-4673-ab2d-62a6888de59f.png)



## Result:
Thus the random classifier was successfully implemented using python programming.

# RANDOM CLASSIFICATION
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Related Theoritical Concept:

## Algorithm
1.In Random forest n number of random records are taken from the data set having k number of records.

2.Individual decision trees are constructed for each sample.

3.Each decision tree will generate an output.

4.Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.

## Program:
```
/*
Program to implement random classification.
Developed by   :Sanjay P
RegisterNumber :  212220230042
*/

import matplotlib.pyplot as plt
from sklearn import datasets
X,y= datasets.make_blobs(n_samples=100,n_features=2, centers=2,cluster_std=1.05,random_state=2)
#plotting
fig =plt.figure(figsize=(10,8))
plt.plot(X[:,0][y == 0],X[:,1][y == 0], 'r^')
plt.plot(X[:,0][y == 1],X[:,1][y == 1], 'bs')
plt.xlabel("feat1")
plt.ylabel("feat2")
plt.title("Random Classification Data with 2 classes")
```

## Output:
![image](https://user-images.githubusercontent.com/75235426/163919085-9654dac1-af5d-4e4c-bd26-c2e05d7b02a2.png)


## Result:
Thus the random classifier was successfully implemented using python programming.

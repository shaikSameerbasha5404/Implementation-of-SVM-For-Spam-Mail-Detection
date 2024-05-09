# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
#### step-1: start.
#### step-2: Import chardet.
#### step-3: Read the dataset.
#### step-4: Import SVC from sklearn.
#### step-5: Fit the data in the model and run the algorithm.
#### step-6: stop.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Shaik Sameer Basha
RegisterNumber:  212222240093

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding="Windows-1252")
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

*/
```

## Output:

#### data.head()
![9 1](https://github.com/shaikSameerbasha5404/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118707756/ce0792be-cc74-4313-81d6-dec04b87dd14)

#### data.tail()
![9 2](https://github.com/shaikSameerbasha5404/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118707756/2b44469d-82ba-4191-8db7-004bf0532e82)


#### data.info()
![9 3](https://github.com/shaikSameerbasha5404/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118707756/5dcd8b78-7aa1-4581-94a0-be6d892744a8)

#### data.isnull().sum()
![9 4](https://github.com/shaikSameerbasha5404/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118707756/bcb12144-7b33-4543-a742-660b83d5958c)

#### Y_prediction value
![9 5](https://github.com/shaikSameerbasha5404/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118707756/2e963ed9-6b5e-49bc-bd8f-fd242fec88f9)

#### Accuracy value
![9 6](https://github.com/shaikSameerbasha5404/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118707756/b4214768-72fb-41cb-8f35-7fbf2e43ab6a)



## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.

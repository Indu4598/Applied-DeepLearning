<h1>Multiclass Classification of Cardiac Arrhythmia </h1>
<h3>Problem Statement: Detection and classification of Arrythmia based on ECG recordings.</h3>

The main aim of the study is to build a system that can classify ECG records into normal and diseased class, i.e., is to distinguish between the presence and absence of cardiac 
arrhythmia and to classify it in one of the 16 groups.

Arrhythmia is a condition in which the heart beats in an irregular fashion, the heart rate can be too fast or too slow. Arrythmia that are not due to structured heart disease 
account for 5 to 10% of sudden cardiac arrests. Early detection of arrythmia can help minimize the human loss. ECG conveys information about the structure and function of 
heart electrical conduction system. It is a graph between the voltage versus time of the electrical activity of the heart. The main components of ECG are 3 waves: P wave, 
QRS wave, and T wave. The Objective of the study is to build different machine learning models and deep learning models to analyze the recordings to detect arrythmia.

The dataset used in this study is “Cardiac Arrythmia Dataset” from UCI Machine Learning Repository. The dataset is ECG recordings of 452 patients.
This database contains 279 attributes, 206 of which are linear valued, and the rest are nominal. The basic features are age, gender, height, and weight of the patient. 
Since the data is about ECG recordings, it contains large number of features like presence of waves like shape, duration and relation between the three different wavs of the ECG. 
The target variable, the variable that need to be predicted has 16 classes. 

<h3>Methods and Results:</h3>
Distribution of Features: 279 attributes, 206 of which are linear valued, and the rest are nominal. Figure1 depicts the distribution of the target variable.
Correlation b/w features:  Figure2 depicts the correlation among the independent variables.
Missing Values: The features which have missing values are features like Vector angles in degrees on front plane of QRS, T, P, QRST, J. These features are linear.
Data Preprocessing: 
1.	Missing Values: In this dataset, the missing values are represented by ‘?’. From preliminary inspection, the features containing missing values are linear. 
The appropriate way to replace missing values is to find the mean of the feature and replace missing value with mean.
2.	Scaling & Encoding: The linear features are normalized before the data is used for training and validation. 
The categorical variables should be one-hot encoded. However, in out data, all the categorical features are binary valued., i.e. 0 and 1.
3.	Data Imbalance: From figure 1, the dataset is imbalanced in terms of target variable. In this study imbalance is handled using two techniques: 
(i) Merge all the disease classes into one class, (ii) combine disease class into smaller sub-groups based on medical terminology. 


<img src="https://github.com/Indu4598/Applied-DeepLearning/blob/main/distribution.png" width="200" />
<img src="https://github.com/Indu4598/Applied-DeepLearning/blob/main/missing.png" width="200" />
<img src="https://github.com/Indu4598/Applied-DeepLearning/blob/main/binary.png" width="200" />
<img src="https://github.com/Indu4598/Applied-DeepLearning/blob/main/mclass.png" width="500" />
<img src="https://github.com/Indu4598/Applied-DeepLearning/blob/main/Binary.png" width="500" />
<img src="https://github.com/Indu4598/Applied-DeepLearning/blob/main/Multiclass.png" width="500" />

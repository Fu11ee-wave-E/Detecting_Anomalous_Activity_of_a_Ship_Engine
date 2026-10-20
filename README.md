# **Detecting Anomalous Activity of a Ship's Engine**
<div align="justify">
  
## **Objectives**

To understand and apply statistical and ML methods for detecting anomalies, where the project:

* explores the data set
* preprocesses the data and conducts feature engineering
* applies statistical techniques to detect anomalies
* uses ML algorithms to detect anomalies.
  
## **Business Context**

Creating a reliable anomaly detection system that assesses engine performance is one 
way to mitigate potential safety hazards and significant downtime that can arise from a 
poorly maintained ship engine. The current study analyses a dataset containing six 
distinct features considered critical to the performance of a ship’s engine. 

## **Methods**

The anomaly detection is initially performed using  a statistical approach incorporating 
the interquartile range (IQR) , followed by two unsupervised machine learning (ML) 
models, namely One-Class Support Vector Machine (SVM) and Isolation Forest (IF). The 
results obtained from the two ML techniques are visualised using a dimensionality 
reduction technique called the Principal Component Analysis (PCA).

## **EDA- Outliers Visualised per Feature**

The colour-coded  box plots produced  for each feature considered critical for engine 
performance:

<br><br>
<p align="left">
  <img src="Figures/boxplots_eda.png" width="800">
</p>
<br><br>

## **IQR Results**

The principle behind the IQR approach is depicted in the figure below where upper and lower 
bounds are derived per feature and used to flag outliers in a row-wise fashion:

<br><br>
<p align="left">
  <img src="Figures/IQR_method.png" width="600">
</p>
<br><br>

The sole presence of an outlier for a given feature does not indicate an anomaly in the 
engine’s status. Therefore, outlier percentage is re-assessed by counting the instances of 
outliers per data entry. As the results in the table below indicate, the total percentage of samples 
identified as outliers falls within the expected 1-5% range only when two features are 
simultaneously flagged.  

<br><br>

## **ML Results**
### **PCA Approach**
### **IF Approach**

<\div>

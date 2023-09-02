# Heart-Attack-Analysis-and-Prediction

**Introduction**

In an era characterized by an increasing focus on preventive healthcare, understanding the factors that contribute to heart attacks and developing effective prediction models has gained paramount importance. This dataset aims to provide researchers, healthcare professionals, and data enthusiasts with a comprehensive collection of features to facilitate in-depth analysis and prediction of heart attacks.


**Describe Dataset:**

**Age :** 
This is a key risk factor for heart disease. As age increases, the risk of damaged and narrowed arteries, weakened or thickened heart muscle, and other heart disease risk factors also increases.

**Sex :** 
Men are generally at higher risk of heart disease than women. However, after menopause, a woman's risk increases to almost match that of a man's.

**Chest Pain Type (cp) :** 
Chest pain is a key symptom of heart disease. It may manifest in different forms: typical angina, atypical angina, non-anginal pain, or may even be asymptomatic. Chest pain associated with heart disease is usually described as a discomfort, heaviness, pressure, aching, burning, fullness, squeezing, or painful feeling.

**Resting Blood Pressure (trtbps) :** 
High blood pressure (hypertension) can harden and thicken arteries, leading to a buildup of plaque (atherosclerosis) that can cause coronary artery disease. The pressure is measured in millimeters of mercury (mm Hg) and is usually recorded as two figures. Normal resting blood pressure in an adult is approximately 120/80 mm Hg.

**Serum Cholesterol (chol) :** 
Cholesterol is a type of lipid molecule. High levels of low-density lipoprotein (LDL) or 'bad cholesterol' can increase the risk of heart disease by forming plaques and narrowing arteries.

**Fasting Blood Sugar (fbs) :** 
High fasting blood sugar levels (prediabetes or diabetes) can contribute to narrowing of the arteries and increase the risk of heart disease. A fasting blood sugar level less than 100 mg/dL is considered normal. 100-125 mg/dL is considered prediabetes, and 126 mg/dL or higher on two separate tests means you have diabetes.

**Resting Electrocardiographic Results (restecg) :** 
ECG records the electrical activity of the heart and can show previous heart attacks or problems with the heart rhythm. Abnormal results can indicate heart conditions such as left ventricular hypertrophy or heart arrhythmias.

**Maximum Heart Rate Achieved (thalachh) :** 
During exercise or stress testing, the maximum heart rate can indicate cardiovascular fitness and the heart's ability to handle exertion.

**Exercise Induced Angina (exang) :** 
This happens when the heart muscle doesn't get as much blood (and thus oxygen) as it needs for the level of physical activity, causing chest pain or discomfort.

**ST Depression Induced by Exercise Relative to Rest (oldpeak) :** 
Changes in the ST segment on an ECG can indicate heart disease. ST depression can indicate ischemia, or lack of sufficient blood flow to the heart muscle.

**The Slope of The Peak Exercise ST Segment (slp) :** 
The ST segment/heart rate slope (ST/HR slope), has been introduced as an index of relative myocardial oxygen demand during exercise. The shape of the ST segment can reveal a lot about the heart's condition.

**Number of Major Vessels Colored by Flourosopy (caa) :** 
This measures the presence of disease in the major blood vessels to the heart. A higher number usually indicates more severe disease.

**Thallium Stress Test (thall) :** 
This is a nuclear imaging method that shows how well blood flows into the heart muscle, both at rest and during activity. It can reveal areas of the heart muscle that aren't receiving enough blood, indicating coronary artery disease.

**Output (Diagnosis of Heart Disease) :** 
This is the target variable. A value of 0 indicates less than 50% diameter narrowing - not a significant heart disease, while a value of 1 indicates more than 50% diameter narrowing - a significant heart disease.


![image](https://github.com/yahyamomtaz/Heart-Attack-Analysis-and-Prediction/assets/95857657/4f0ec82c-6a6c-4167-a0a2-74ff42e4aebf)

![image](https://github.com/yahyamomtaz/Heart-Attack-Analysis-and-Prediction/assets/95857657/77c571c9-646f-4504-8a75-d66cd876deb4)

![image](https://github.com/yahyamomtaz/Heart-Attack-Analysis-and-Prediction/assets/95857657/fd5df7e8-9810-416e-9211-d4e28aca9f5c)

![image](https://github.com/yahyamomtaz/Heart-Attack-Analysis-and-Prediction/assets/95857657/563886db-b041-4b45-beb1-b1880714f75b)

![image](https://github.com/yahyamomtaz/Heart-Attack-Analysis-and-Prediction/assets/95857657/4cc6911c-2543-4827-9469-b3e5ae7c47c8)


**Describe the outcome:**

Patients who have chest pain have a higher risk of developing heart disease. This statement aligns with medical knowledge. Chest pain, especially if it occurs during physical exertion (such as exercise-induced angina), can be a significant symptom of coronary artery disease (CAD) or other heart-related conditions. Chest pain may indicate that the heart is not receiving an adequate blood supply, which can be a warning sign of heart disease.

An increased chance of heart disease is linked to a high maximum heart rate obtained during testing. A high maximum heart rate during exercise testing can be indicative of an increased risk of heart disease. It may suggest that the heart is under stress during physical activity and may not be functioning optimally. However, this should be interpreted in the context of the individual's age, fitness level, and other clinical factors. A high maximum heart rate alone is not a definitive indicator of heart disease but can be a valuable diagnostic clue.

patients who have downsloping peak exercise are more linked to the heart diseases. The term "downsloping peak exercise" typically refers to certain patterns observed on an electrocardiogram (ECG or EKG) during exercise stress testing. These patterns can sometimes be associated with an increased risk of heart disease, particularly coronary artery disease. They may indicate abnormal electrical activity or blood flow in the heart during physical exertion.

Individuals who experience exercise-induced angina(exang) may have a reduced risk of heart disease compared to those who do not experience this symptom during exercise. Exercise-induced angina is typically a symptom of coronary artery disease (CAD) or reduced blood flow to the heart muscle during physical exertion. it's(exang) negatively correlated with heart disease in dataset, it might indicate that this symptom is acting as a protective factor or an early warning sign for individuals, leading to earlier diagnosis and management of heart-related conditions.

There is a negative correlation between ST Depression Induced by Exercise Relative to Rest(oldpeak) and heart disease in dataset, it implies that as the magnitude of ST depression induced by exercise relative to rest increases, the risk of heart disease tends to decrease, and vice versa. However, interpreting this correlation requires caution and consideration of other factors. ST depression during exercise, often seen on an electrocardiogram (ECG or EKG), can sometimes be a sign of cardiac ischemia or insufficient blood flow to the heart muscle during physical exertion. In many cases, ST depression can be indicative of underlying heart problems.

**Classification**

We are going through to build and evaluate 4 different machine learning models (Decision Tree, Support Vector Machine - SVM, Logistic Regression, and k-Nearest Neighbors - k-NN) for our dataset in the following steps:

1. Data Preprocessing
2. Model Building
3. Model Evaluation
4. Model Comparison
5. Conclusion

![image](https://github.com/yahyamomtaz/Heart-Attack-Analysis-and-Prediction/assets/95857657/26fb8653-46d2-4387-8d9d-a8c7a4e02f5d)

**Conclusion**

**Decision Tree:** The Decision Tree model exhibits solid performance with an accuracy of approximately 88.21% on the training set and 85.71% on the test set. It demonstrates its ability to generalize to unseen data while maintaining a high level of accuracy.

**SVM:** The Support Vector Machine (SVM) model shows promising results, achieving an accuracy of approximately 85.54% on the training set and an even better 90.16% on the test set. Additionally, the model's F1-score and Jaccard score are both strong, indicating a robust ability to classify cases accurately.

**Logistic Regression:** Logistic Regression performs well with an accuracy of around 86.79% on the training set. However, its accuracy slightly drops to 80.22% on the test set. The F1-score and Jaccard score, though slightly lower than SVM, suggest that it still provides reasonable predictive capabilities.

**K-Nearest Neighbors (KNN):** The KNN model achieves an accuracy of approximately 85.12% on the training set and maintains a consistent performance on the test set with an accuracy of 85.25%. This demonstrates the model's stability and reliability in classifying instances.

In summary, each model shows promise in its ability to predict heart disease. SVM appears to be the top performer in terms of accuracy, F1-score, and Jaccard score on the test set. However, the Decision Tree, Logistic Regression, and KNN models also provide respectable results. The choice of the best model may depend on various factors, including the specific requirements of our application and the trade-offs between different evaluation metrics. Further fine-tuning and validation may help in making a final model selection.


For more details open .ipynb file


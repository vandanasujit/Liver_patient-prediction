## Dataset Link:
### Context
Patients with Liver disease have been continuously increasing because of excessive consumption of alcohol, inhale of harmful gases, intake of contaminated food, pickles and drugs. This dataset was used to evaluate prediction algorithms in an effort to reduce burden on doctors.
### Content
This data set contains 416 liver patient records and 167 non liver patient records collected from North East of Andhra Pradesh, India. The "Target" column is a class label used to divide groups into liver patients (liver disease) or not (no disease). This data set contains 441 male patient records and 142 female patient records.
Any patient whose age exceeded 89 is listed as being of age "90".
### Domain: Healthcare
### Attribute information:
●	Age of the patient
●	Gender of the patient
●	Total Bilirubin
●	Direct Bilirubin
●	Alkaline Phosphotase
●	Alamine Aminotransferase
●	Aspartate Aminotransferase
●	Total Protiens
●	Albumin
●	Albumin and Globulin Ratio
●	Target: field used to split the data into two sets (1 : patient with  liver disease and 2: patient with no liver disease disease)

### Link : https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1007-LiverPatientPred.zip


## Challenges faced in this project:
-----------------------------------
### * Imbalanced dataset:
The dataset was highly imbalanced, with a majority of patients having liver disease (class 1) and a minority of patients not having the disease (class 2).To address this imbalance, we applied balancing techniques such as oversampling the minority class to improve the model's ability to predict both classes accurately.
### * Feature Scaling:
The features had varying ranges, which could affect the performance of distance-based models. We used StandardScaler to normalize the features, ensuring that all features contributed equally to the model’s predictions.:
### * Overfitting:
The model tended to overfit on the training data, particularly when using tree classifiers leading to poor generalization on the test data. so we applied tuning hyperparameters to control the model complexity and reduce overfitting.
### * Feature Selection:
Identifying the most important features that contribute to predicting liver disease was crucial but challenging. We performed exploratory data analysis (EDA)n heatmap and correlation matrix to ensure that the right features were used in the model.
### * Choosing the Right Model:
Selecting a model that could handle the imbalanced data and perform well across both classes required extensive experimentation. We tested several classification algorithms including distance-based algorithms and tree based algorithms and found out Random Forest gave the best result for this dataset.

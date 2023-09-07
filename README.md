# breast_cancer_predictor_kyrgyzstan
Topic: Medical data analysis for predicting BIRADS (breast imaging assessment category): Utilizing machine learning.

About the Data

In the structure of oncological diseases in the Kyrgyz Republic, breast cancer occupies the first place, accounting for 18.5%. In 2020, a total of 615 new cases of breast cancer were registered. Breast cancer also ranks first in the mortality structure (8.9%). At this form of cancer, stages 3 and 4 are considered advanced, with their indicators being 26.5% and 12.4%, respectively. This means that 38.9% of new breast cancer cases are detected at late stages.

The data were collected within the project "Early Diagnosis of Breast Cancer and Cervical Cancer in the Kyrgyz Republic using a Mobile Mammographic Center", initiated by the "Ergene" Public Fund, with the aim of providing equitable access to early diagnosis of common types of cancer in women in the regions using high-tech methods.

The goal of this project is to study women's health for breast cancer, which is the leading cause of morbidity and mortality among oncological diseases in our country.

Data Analysis

Medical science extensively utilizes the advantages of modern data processing methods and machine learning for predicting various diseases and diagnosing patients. This article presents a study where we explored data analysis methods of a pre-processed data set about women undergoing mammography. In this article, we focused on predicting BIRADS (Breast Imaging Reporting and Data System) based on medical histories and mammographic images. BIRADS is a classification system of mammographic results that helps doctors standardize and describe patterns of breast changes detected.
Before the data analysis, we conducted thorough cleaning, outlier removal, and filling in missing values. Then we performed data visualization using Python libraries for a deeper understanding of feature distribution and dependencies between them.
In this article, we utilized visualization to highlight key aspects of the data and identify important features that could influence the prediction of BIRADS categories. Visualization allows for a clear representation of data structure, revealing patterns and correlations between features, and identifying outliers or anomalies that might affect prediction quality.
Through visualization, we can analyze the relationships between various parameters of medical histories and mammographic images with the BIRADS category. For instance, it is possible to highlight specific characteristics that are more commonly found in patients with different BIRADS categories. This can help identify important features that can be used to improve prediction accuracy and assist doctors in making more informed decisions.
Using visualization in data research significantly aids in understanding data structure, identifying patterns, and gathering insights that can be used to develop more effective BIRADS prediction models and improve diagnostic quality.
In the next stage, we applied several machine learning models, such as Logistic Regression, Random Forest Classifier, Gradient Boosting Classifier, and Cat Boost Classifier. To obtain a more objective evaluation of the model performance, we applied several approaches and performance evaluation methods.
The results of this research can be used in medical practice for more effective and accurate diagnosis of breast cancer in women. However, to get a more complete picture and to apply the models in practice, it is recommended to conduct additional research on larger data sets and to test the models on new patients to verify their effectiveness in real conditions.

On the evaluation system used in reading mammographic images.
BI-RADS assessment categories and their corresponding recommendations:
Category 0 – incomplete data, unable to reach a conclusive conclusion from the visualization results, further examination is necessary. This category is only valid for screening examinations.
Category 1 – normal mammography results. No formations, architectural disturbances, or suspicious calcifications.
Category 2 – unequivocally benign changes.
Category 3 – most likely a benign formation (up to 98% chance that it's a benign process), control visualization of changes in 6 months – mammography of one breast, meanwhile, the category remains 3. Later, with a stable picture, mammography of both breasts is recommended after 12 months. With a stable picture of identified changes, the category changes to 2 and control is scheduled in 12 months. This is a borderline category with dynamic control following the 6-12-12 months scheme.
Category 4 – changes detected on mammograms are suspicious for a malignant process with a probability ranging from 2 to 94%:
low probability, from 2 to 10% - BI-RADS 4a;
medium (moderate) probability, from 10 to 50% - BI-RADS 4b;
high probability, from 50 to 95% - BI-RADS 4c.
Assignment of this category requires morphological verification through stereotactic core biopsy.
Category 5 – malignant changes are likely, all identified signs indicate the presence of breast cancer.
Category 6 – unequivocally malignant changes. This category includes patients with an already verified diagnosis of a malignant process in the breast.














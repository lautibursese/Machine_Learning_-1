

​
# <h1 align="center">**`Machine Learning`**

<p align="center">
<img src="https://www.paho.org/sites/default/files/styles/max_1500x1500/public/2022-12/dsc8197.jpg?itok=JO8szoc-"   
>
</p>

​

## 🏥 **Hospital stay** 🏥

Hospitalization, or hospital stay, when it is prolonged, is a worldwide concern due to its negative effects on the health system, increasing costs, generating deficiency in the accessibility of health services, saturation of hospitalization and emergency units. Consequently, greater adverse effects such as hospital-acquired diseases.

The study of health care processes, as well as the knowledge of the characteristics and profiles of users with the aim of predicting hospital occupancy, is one of the aspects in which the health authorities have paid great interest, since it allows not not only guarantee the necessary resources for patient care, but also make adjustments regarding the supply and demand of health services and associated implements.
​
## **Description of the problem**

An important Health Center has hired him in order to predict whether a patient will have a prolonged hospital stay or not, using the information contained in the associated dataset, which collects a historical sample of its patients, in order to manage the demand for beds in the hospital according to the condition of recently admitted patients.

For this, a patient is defined as having a prolonged hospital stay if they have been hospitalized for more than 8 days. Therefore, you must generate said categorical variable and then categorize the patients according to the variables that you consider necessary, justifying said choice. 
​
Remember to verify that the number of columns of the data set that you use to train the model is the same as the number of columns that the test set has, with which you will make the predictions.

## **Evaluation criteria**
The proposed solution will include:

- Training and prediction using a Machine Learning Model appropriate to the problem (classification or regression).
- Exploratory data analysis (EDA).
- Split dataset into train and test using train_test_split, CV, KFold or similar.
- Comments and writing with the justification of the proposed solution, written in Markdown in the Jupyter Notebook (.ipynb) or in a separate document.

​
## **Metric to use**
​
As a method of evaluating the performance of the model, the Recall metric will be used for long hospital stays, based on the confusion matrix (Confusion Matrix).


$$ Recall=\frac{TP}{TP+FN}$$


Where $TP$ are the true positives and $FN$ the false negatives.

As an additional metric to check the performance of your model, the Accuracy metric will also be used for long hospital stays.

$$ Accuracy=\frac{TP+TN}{P+N}$$

being $TP$ true positives, $TN$ true negatives and $P+N$ total population.


​
## **Files**
​
The following files are provided to carry out the project:
 - 'hospitalizaciones_train.csv': Contains 410000 records and 15 dimensions, which includes **numeric** information on the number of days of hospital stay.
 - 'hospitalizaciones_test.csv': Contains 90,000 records and 14 dimensions, which does not include information on the number of days of hospital stay.
​
## **Dimension Description**
- Available Extra Rooms in Hospital: Additional rooms available in the hospital. A room is not the same as a patient, they can be individual or shared.
- Department: Service area to which the patient enters.
- Ward_Facility_Code: Code of the patient's room.
- doctor_name: Name of the doctor in charge of the patient.
- staff_available: Number of staff available at the time of patient admission.
- patientid: Patient identifier.
- Age: Age of the patient.
- gender: Gender of the patient.
- Type of Admission: Type of admission registered according to the patient's admission situation.
- Severity of Illness: Severity of the disease/condition/state of the patient at the time of admission.
- health_conditions: Health conditions of the patient.
- Visitors with Patient: Number of registered visitors for the patient.
- Insurance: Indicates whether or not the person has health insurance.
- Admission_Deposit: Payment made on behalf of the patient, in order to cover the initial hospitalization costs.
- Stay (in days): Recorded days of hospital stay.
​
## **EDA includes:**
- Pandas first impression (info)
- Pandas describe
- Seaborn barplot
- Seaborn countplot
- Seaborn boxplot

## **Conclusion**
The Random Forest model trained on hospital data shows promising results with an accuracy of 0.76 and precision, recall, and F1 score of over 0.78, 0.84, and 0.81 respectively. These statistics indicate that the model can be used as a helpful tool in hospitals for identifying patients who are at a higher risk of developing certain medical conditions.

By using the trained model, hospital staff can prioritize patients who need further medical attention and resources, ultimately leading to better health outcomes and efficient use of resources. Additionally, the model can be updated and trained on new data regularly to keep it up-to-date and accurate in predicting medical conditions.

In conclusion, the Random Forest model has the potential to improve patient outcomes and resource allocation in hospitals, making it a valuable tool in the healthcare industry.
🩺 Health Prediction App Suite
A collection of Streamlit-based machine learning web apps for predicting Diabetes, Heart Disease, and Breast Cancer using trained models and medical datasets.

📂 Apps Included
1. Health Prediction App (app2.py)
Predicts the risk of Diabetes and Heart Disease based on user-provided health parameters.

🧪 Diabetes Model:

Input Features: Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age

Output: Probability and binary classification for diabetes

❤️ Heart Disease Model:

Input Features: Age, Sex, Chest Pain Type, Blood Pressure, Cholesterol, Fasting Blood Sugar, Resting ECG, Max Heart Rate, Exercise Angina, Oldpeak, ST Segment Slope

Output: Probability and binary classification for heart disease

📊 Built-in visualizations of user input values using Plotly

2. Breast Cancer Prediction App (breast_cancer_app.py)
Predicts whether a tumor is malignant or benign based on 30 input features.

🔬 Uses the sklearn.datasets.load_breast_cancer dataset

🧠 Model: Logistic Regression

💡 Input: 30 numerical medical features from user

📈 Output: Malignant/Benign prediction with confidence scores

🛠️ Requirements
Make sure you have the following Python libraries installed:

bash
Copy
Edit
pip install streamlit scikit-learn pandas numpy plotly
▶️ Running the Apps
Run any of the apps using Streamlit:

bash
Copy
Edit
streamlit run app2.py
or

bash
Copy
Edit
streamlit run breast_cancer_app.py
📁 Project Structure
text
Copy
Edit
.
├── app2.py                      # Streamlit app for diabetes and heart disease prediction
├── breast_cancer_app.py         # Streamlit app for breast cancer prediction
├── check.py                     # Script to check features of random forest model
├── diabetes_model.pkl           # Trained model for diabetes
├── heart_model.pkl              # Trained model for heart disease
├── breast_cancer_svm_model.pkl  # SVM model for breast cancer (not used in main app)
├── *.csv                        # Dataset files used for training and testing
🧠 Model Training
Models were trained using scikit-learn on relevant datasets:

diabetes_model.pkl: Trained on PIMA diabetes dataset

heart_model.pkl: Trained on heart disease UCI dataset

breast_cancer_svm_model.pkl: Optional SVM model for breast cancer (not deployed in main UI)

📌 Features
🖼️ Interactive sliders, number inputs, and dropdowns for user-friendly input

🔐 Local model loading via pickle

📉 Visualizations with Plotly

🧾 Model probability outputs for better interpretability

🚀 Future Improvements
Add model selection toggle for different algorithms (e.g., SVM, Random Forest)

Implement multi-class classification if applicable

Add authentication and session saving

Improve UI styling

Made with 💙 using Streamlit and Scikit-learn.

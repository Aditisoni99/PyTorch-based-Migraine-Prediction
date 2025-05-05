# PyTorch-based-Migraine-Prediction
This project explores the use of deep learning to predict migraine subtypes based on patient-reported symptoms. Built in collaboration with a computational EEG researcher, our goal was to understand how structured clinical features — like nausea, photophobia, and intensity — could be used to assist diagnosis and classification of migraine types.
Project Motivation: 
Migraines affect millions and are often misclassified due to overlapping symptoms. In collaboration with a friend from the Communication Science department (specializing in computational EEG), we became curious about how structured symptom data and future EEG integration could assist migraine diagnosis. This project is the first step toward that vision.

Dataset Overview: 
The dataset contains anonymized patient records with features including:
Demographics: Age, Duration, Frequency
Symptoms: Photophobia, Phonophobia, Nausea, Vomiting, etc.
Target: Migraine type classification (e.g., Typical aura with migraine)

🔬 Exploratory Data Insights:
The age group 20–30 is the most affected.
The typical aura with migraine is the most common type.
Strong correlations between symptoms like photophobia, phonophobia, and nausea.

Visualizations attached:
![image](https://github.com/user-attachments/assets/e20262c0-bccf-4451-990f-ebde7a669376)
![image](https://github.com/user-attachments/assets/13f6fd31-d3c9-4e56-9ae2-941ecdf3ed5f)
![image](https://github.com/user-attachments/assets/9fdcb979-1890-406c-9171-1fb0e925df39)

Model Architecture:
Built with PyTorch
3-layer fully connected neural network
ReLU activations, CrossEntropyLoss
Preprocessing with Scikit-learn (StandardScaler, LabelEncoder)

Task: Multi-class classification of migraine types

Results:
Accuracy: 91%
Macro Average F1-score: 0.77
Weighted Average F1-score: 0.90

Confusion Matrix:
![image](https://github.com/user-attachments/assets/1204532a-d3f2-40e5-97c6-318b2aa7205b)

Classification Report: These results indicate strong performance in identifying the most common migraine types while revealing an opportunity to improve on rarer classes through future data augmentation.

Future Work
Add EEG data for multimodal input
Expand dataset for better generalization
Deploy as a clinical tool for real-time support


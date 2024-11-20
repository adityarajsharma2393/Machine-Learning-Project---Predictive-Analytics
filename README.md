Teach For America Recruitment Optimization
This repository contains the final project for MAX 522 - Predictive Analytics, led by Aditya Raj Sharma, focusing on predictive modeling to enhance recruitment strategies for Teach For America (TFA). The project employs various machine learning models to predict applicant outcomes and optimize resource allocation.

Project Overview
Teach For America (TFA) faces challenges in maintaining application rates, threatening its mission to empower underserved schools. This project uses predictive analytics to identify candidates likely to complete the admission process, enabling TFA to improve recruitment efficiency.

Data Overview
The dataset includes 37,134 rows and features variables such as:

Applicant academic performance (e.g., GPA).
Engagement metrics (e.g., essay attributes, event attendance).
Application timelines and outcomes.
Objectives
Predict completion of the admission process (completedadm).
Compare machine learning models to determine the most effective for TFA's recruitment needs.
Models Evaluated
The following models were tested and fine-tuned:

k-Nearest Neighbors (kNN): Achieved accuracy up to 83.73% with k=5.
Naive Bayes: Demonstrated moderate accuracy (76.6%) with text-focused features.
Decision Trees (C5.0): Selected as the optimal model with an accuracy of 79.86%.
Artificial Neural Networks (ANN): Showed potential but faced convergence issues.
Support Vector Machines (SVM): Provided limited success, heavily biased towards positive predictions.
Key Results
Decision Trees with 8 trials emerged as the most suitable model for TFA due to:
Balanced accuracy across true positives and negatives.
High interpretability for decision-making.
Better handling of class imbalance.


.
├── data/                     # Dataset used for training and testing
├── scripts/                  # Code for model implementation and evaluation
│   ├── knn.R                 # k-Nearest Neighbors implementation
│   ├── naive_bayes.R         # Naive Bayes implementation
│   ├── decision_trees.R      # Decision Trees implementation
│   ├── ann.R                 # Artificial Neural Networks implementation
│   ├── svm.R                 # Support Vector Machines implementation
├── results/                  # Model results and confusion matrices
├── README.md                 # Project documentation (this file)
└── report.pdf                # Final project report

How to Run
Clone the repository:
bash
Copy code
git clone https://github.com/your-repo/teach-for-america-recruitment.git
cd teach-for-america-recruitment
Install required libraries in R:
R
Copy code
install.packages(c("class", "e1071", "C50", "neuralnet", "kernlab", "caret", "gmodels"))
Run the scripts for individual models located in the scripts/ directory.
Recommendations
Adopt the Decision Trees model with 8 trials for robust and interpretable predictions.
Continue refining data preprocessing, particularly addressing class imbalances for improved outcomes.
Acknowledgments
This project was developed under the guidance of Dr. Dinakar Jayarajan. Special thanks to Teach For America for providing the dataset and context for this predictive analytics study.

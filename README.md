# 🏥 Medicine Recommendation System

## 🩺 Project Overview
The Medicine Recommendation System predicts diseases based on a user’s symptoms and recommends suitable medications, diets, precautions, and workouts. The system uses multiple machine learning models and provides an easy-to-use interface for users to input symptoms and get disease predictions with relevant recommendations.

## ✨ Features
🔍 Disease Prediction: Predicts the disease based on symptoms using trained machine learning models like Support Vector Machine (SVM) and Random Forest (RF).
💊 Recommendations: Provides recommendations such as medications, precautions, diets, and workout plans based on the predicted disease.
🤖 Models: Includes various classifiers like Random Forest, Gradient Boosting, Naive Bayes, K-Nearest Neighbors, and Support Vector Machine.
🗄️ Data Handling: Manages different data sources like symptoms, disease descriptions, medications, precautions, and more.
🌐 Web Application: Built with Flask to provide an interactive user interface for entering symptoms and viewing predictions

## 🔄 Workflow

#### Data Preprocessing:
🧹 The dataset containing symptoms and corresponding diseases is cleaned and prepared.
🎯 The target variable (disease) is encoded using LabelEncoder.

#### Model Training:
🧑‍💻 Several machine learning models are trained using train_test_split (70% training, 30% testing).
🏅 Models include RandomForest, SVM, KNeighborsClassifier, MultinomialNB, and GradientBoostingClassifier.
📈 Accuracy and confusion matrices are evaluated for each model.

#### Model Persistence:
💾 The best-performing models (Random Forest and SVM) are saved using the pickle module for future predictions.

#### Symptom Prediction:
📝 Users input their symptoms as comma-separated values.
🔮 The system matches the symptoms to a disease using the trained SVM model and provides detailed recommendations.

#### Recommendations:
💊 Once the disease is predicted, recommendations related to medications, diets, workouts, and precautions are retrieved from preloaded CSV datasets.

#### Web Interface:
🌐 The Flask web application provides a simple user interface where users can input symptoms, and the system predicts the disease and displays the corresponding recommendations.

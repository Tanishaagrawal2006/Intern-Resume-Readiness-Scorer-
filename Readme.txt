Intern Portfolio Readiness Scorer:

The Intern Portfolio Readiness Scorer is a machine learning based web application that helps students and freshers check how ready their resume is for internship opportunities.

This project analyzes resumes and predicts internship readiness using ML models. It provides:

******************************** index.html ***************************************

Resume quality score:

--> ATS score
--> Skills match percentage
--> Internship readiness prediction
--> Improvement suggestions
--> Resume comparison reports

The platform is mainly designed for:

--> Students
--> Freshers
--> Internship applicants
--> MCA/BCA/BTech graduates

****** Project Purpose ******

Many students apply for internships without knowing:

-->  Whether their resume is strong enough
-->  If their skills match the target role
-->  What improvements are needed
-->  Whether their profile is ATS friendly

This project solves that problem using machine learning and resume analysis techniques.

Main Features:

1. Resume Upload System : Users can upload resumes directly from the website.

Supported features:

-->  Resume upload
-->  Drag and drop support

PDF resume support : Multiple resume upload for comparison

2. Machine Learning Based Prediction

The project uses machine learning models to predict internship readiness.

The ML system analyzes:

--> Skills
--> Projects
--> Resume structure
--> Keywords
--> ATS compatibility
--> Internship role matching

The model predicts:

Readiness score
Internship fit level
Resume strength
Machine Learning Models Used

The project uses:

Logistic Regression
Random Forest Classifier
Decision Tree Classifier

These models help generate accurate readiness predictions.

****** ML Workflow ******

--> Step 1 – Resume Upload : User uploads the resume.
--> Step 2 – Text Extraction : Resume text is extracted from the uploaded file.
--> Step 3 – Feature Engineering : Important resume features are identified such as:

Technical skills

--> Project count
--> Certifications

Keywords : Resume quality indicators

-->  Step 4 – Model Prediction : The trained ML model predicts:

    Internship readiness percentage
    ATS score
    Skills match score

--> Step 5 – Final Report : The user receives:

Readiness analysis
Suggestions
Improvement feedback
Resume Comparison Feature

Users can compare two resumes side-by-side.

The comparison system checks:

--> Resume quality
--> ATS score
--> Skills match
--> Internship fit
--> Missing skills
--> Target Internship Selection

Users can select internship tracks such as:

--> Data Analytics Intern
--> Web Development Intern
--> Backend Developer Intern
--> Frontend Development Intern
--> UI/UX Design Intern
--> Graphic Design Intern

The prediction system changes according to the selected role.

****** GitHub Integration ******

Users can optionally enter their GitHub username.

This helps in:

--> Portfolio evaluation
--> Developer profile analysis
--> Project consistency checking


View History Feature : The project stores previous reports using MongoDB.

Users can:

View old reports
Track improvement
Compare past scores
Technologies Used
Frontend
HTML5
CSS3
JavaScript
Backend
Python
Flask
Machine Learning
Scikit-learn
Pandas
NumPy
Database
MongoDB
Icons & UI
Font Awesome
User Interface Sections
Navigation Bar

Contains:

How It Works
Features
About
Resume Readiness Checker
Resume Comparison
View History
Hero Section

Displays:

Internship readiness overview
Readiness score preview
Platform introduction

Three Quick Steps

--> Step 1 – Upload Resume : Users upload their resume.
--> Step 2 – Resume Analysis : The system analyzes: Resume quality,Skills,ATS compatibility,Keywords
--> Step 3 – Get Suggestions : The system provides improvement recommendations.

Features Section

The platform checks:

Resume quality
Resume readability
Skills and projects
Role-based keyword matching
Portfolio consistency
Internship fit
Example Result Dashboard

The platform displays:

Readiness percentage
ATS score
Skills match
Resume quality
Match level
Statistics Section

The homepage shows:

Total profiles analyzed
ATS improvement percentage
Average analysis time
Responsive Design

The website works on:

Desktop
Tablet
Mobile devices

Media queries are used for responsive layouts.

JavaScript Functionalities

The project includes:

Smooth scrolling
File upload handling
Resume comparison toggle
Animated counters
Progress bar animations
Scroll reveal animations
Dynamic UI updates
Fetch API integration
Backend Integration

The frontend sends form data to Flask backend using:

fetch('/analyze', {
    method: 'POST',
    body: formData
})

The backend performs:

Resume parsing
Feature extraction
ML prediction
ATS scoring
Recommendation generation
MongoDB Usage

MongoDB is used to:

Store history
Save reports
Manage analysis records
Design Highlights
UI Design
Dark theme dashboard
Neon green highlight colors
Modern card layout
Animations
Hover effects
Card tilt effect
Circular progress animations
Counter animations
Scroll reveal animations
Future Improvements

Future updates may include:

AI resume suggestions
LinkedIn profile integration
Real-time internship recommendations
PDF report generation
AI interview preparation
Skill gap analysis
Project Benefits

This project helps students:

Improve resumes
Understand internship requirements
Increase ATS compatibility
Build stronger portfolios
Prepare for placements

************************************** app.py **************************************

This project also uses Machine Learning (ML) model prediction to calculate the candidate readiness score.
The system combines rule-based ATS analysis with ML-based prediction for more accurate resume evaluation.

Technologies and concepts used in the project include:

--> Flask Framework
--> MongoDB Database Integration
--> Machine Learning Model Prediction
--> Joblib Model Loading
--> Pandas & NumPy for Data Processing
--> Resume ATS Scoring System
--> GitHub Profile Analysis
--> PDF and DOCX Resume Parsing
--> Dynamic Skill Matching Engine
--> Role-Based Recommendation System
--> Resume Comparison System
--> Data Visualization Metrics
--> REST-based Application Flow

**** The ML model predicts candidate readiness based on features such as: ****

--> Skills detected
--> Number of projects
--> GitHub repository count

*** Tool usage ***
--> Resume structure
--> Internship role mapping
--> Technical keyword density

*** Final scores are generated by combining: ***
--> ATS Rule-Based Score
--> Skill Match Score
--> Interest Match Score
--> ML Prediction Score

This helps provide smarter and more accurate resume analysis and candidate recommendations.

************************************resume_analyzer.py********************************

The resume_analyzer.py module is the core resume processing and evaluation engine of the project.
It performs resume parsing, OCR extraction, ATS analysis, role-based skill matching, and intelligent resume scoring.

Main functionalities implemented in this module:

--> PDF Resume Text Extraction using pdfplumber
--> DOCX Resume Parsing using python-docx
--> OCR-based Image Resume Scanning using pytesseract
--> Scanned PDF OCR Processing using pypdfium2
--> Candidate Email Extraction
--> Phone Number Detection
--> Automatic Candidate Name Detection
--> Dynamic Skill Matching Engine
--> Multi-Role Resume Classification
--> ATS Optimization Scoring
--> Resume Quality Evaluation
--> Resume Completeness Analysis
--> Technical Keyword Detection
--> Missing Skill Gap Analysis
--> Role Recommendation System
--> Structured Resume Parsing
--> Resume Fit Classification

The system supports multiple internship domains including:

--> Data Analytics
--> Web Development
--> Graphic Design
--> UI/UX Design
--> Backend Development
--> Frontend Development

Advanced features used in the analyzer:

--> OCR fallback system for scanned resumes
--> Regex-based intelligent parsing
--> Dynamic ATS section validation
--> Strict keyword boundary matching
--> Automated score balancing algorithm
--> Resume structure verification
--> Contact information validation
--> Technical project detection
--> Portfolio and GitHub profile validation

Scoring Parameters Used:

--> Skill Match Score
--> ATS Optimization Score
--> Resume Quality Score
--> Profile Completeness Score

Final resume score is calculated using a weighted scoring formula to generate accurate candidate 
evaluation and internship readiness analysis.

************************************** compare_result.html ******************************************

This HTML template is designed for the Dual Resume Comparison Dashboard of the Resume Analyzer project.
It provides a modern matrix-based UI to compare two resumes side-by-side using dynamic evaluation metrics.

Main functionalities implemented in this template:

--> Dual Resume Comparison Interface
--> Dynamic Candidate Score Visualization
--> Skill Match Matrix Display
--> Resume Quality Analysis
--> Profile Completeness Tracking
--> ATS Optimization Score Visualization
--> Technical Skill Badge Rendering
--> Real-Time Resume Evaluation Output
--> Role-Based Resume Comparison
--> Flask Template Rendering using Jinja2
--> Responsive Grid-Based Layout
--> Dynamic Progress Bar Indicators
--> Internship Readiness Comparison System

Frontend technologies used:

--> HTML5
--> CSS3
--> Flask Jinja2 Templating Engine
--> Dynamic Inline Styling
--> Responsive Layout Design

UI Features included:

--> Dark Theme Dashboard
--> Animated Progress Bar Style Layout
--> Candidate Comparison Cards
--> Dynamic Percentage Indicators
--> Skill Detection Tags
--> Structured Resume Analytics Panel
--> ATS Structural Alignment Visualization
--> Interactive Resume Evaluation Matrix

Dynamic variables rendered from Flask backend:

r1.best_score
r2.best_score
r1.skill_match
r2.skill_match
r1.quality
r2.quality
r1.completeness
r2.completeness
r1.ats_score
r2.ats_score
skills_matched
candidate_name
target_role

The dashboard helps recruiters and users compare resumes efficiently by visualizing candidate 
strengths, ATS compatibility, and technical skill alignment in a structured analytical format.

************************************ result.html *********************************************

This file is the main result dashboard template of the Intern Portfolio Readiness Scorer system.
It is built using HTML, CSS, and Jinja templating for dynamic rendering inside the Flask framework.

Main Functionalities:

--> Displays the final resume evaluation score using an animated circular progress indicator
--> Shows candidate details and target internship role

Generates fit status labels such as:
--> Strong Fit
--> Moderate Match
--> Needs Improvement

Visualizes:
--> Skill Match Score
--> Resume Quality Score
--> Profile Completeness
--> ATS Optimization Score

Displays:
--> Matched keywords
--> Missing keywords
--> Structural gaps in resume
--> Personalized improvement suggestions
--> Dynamically loads GitHub repositories using GitHub API integration
--> Uses responsive UI design for desktop and mobile compatibility
--> Implements animated progress bars and modern dashboard styling
--> Supports Flask-Jinja variables for real-time data rendering

Technologies Used:
--> HTML5
--> CSS3
--> Flask Jinja2 Template Engine
--> Responsive Grid Layout
--> SVG Circular Progress Animation

Key UI Features:
--> Dark futuristic dashboard theme
--> Animated score visualization
--> Responsive design
--> Dynamic portfolio keyword matrix
--> GitHub repository cards
--> ATS tracking visualization

Purpose:

This template provides a professional AI-style resume evaluation interface that helps users 
understand:
--> Resume strengths
--> Missing technical skills
--> ATS readiness
--> Portfolio quality
--> Overall internship readiness score

******************************** benchmark_models.py *****************************************

This file is responsible for benchmarking and evaluating multiple Machine Learning classification models used in the Graphura Resume Readiness Scorer system.

Main Functionalities:
--> Loads and preprocesses resume dataset from CSV files
--> Cleans and prepares structured internship readiness data
--> Splits dataset into training and testing sets
--> Builds preprocessing pipelines for:
    --> Numerical features
    --> Categorical features

Applies:
--> Missing value handling
--> Feature scaling
--> One-hot encoding

Trains and compares multiple ML models:
--> Logistic Regression
--> Decision Tree Classifier
--> Random Forest Classifier

Calculates important evaluation metrics:
--> Training Accuracy
--> Testing Accuracy
--> Balanced Accuracy
--> Weighted F1 Score
--> Overfitting Gap

Generates a benchmark comparison table
Exports benchmark results into CSV reports

Machine Learning Workflow:
--> Dataset loading
--> Feature preprocessing
--> Train-test splitting
--> Pipeline creation
--> Model training
--> Prediction generation
--> Performance evaluation
--> Accuracy comparison reporting

Technologies & Libraries Used:
--> Python
--> Pandas
--> Scikit-learn
--> NumPy
--> Pipeline API
--> ColumnTransformer
--> Logistic Regression
--> Decision Tree
--> Random Forest

ML Concepts Implemented:
--> Feature Engineering
--> Data Preprocessing
--> Classification Modeling
--> Model Benchmarking
--> Performance Evaluation
--> Overfitting Detection
--> Data Transformation Pipelines

Output Generated:
--> model_accuracy_table.csv
--> Console-based benchmark report
--> Accuracy comparison matrix

Purpose:

This module helps identify the best-performing machine learning model for predicting internship
portfolio readiness by comparing multiple algorithms using standardized evaluation metrics.

Key Features:
--> Automated preprocessing pipeline
--> Dynamic dataset loading
--> Structured ML benchmarking
--> Overfitting analysis
--> Exportable evaluation reports
--> Multi-model comparison system

*********************************** extract_features.py ****************************************

This file is responsible for extracting, cleaning, preprocessing, and transforming structured resume dataset features for the Graphura Resume Readiness Scorer machine learning pipeline.

Main Functionalities:
--> Loads processed internship resume dataset from CSV files
--> Cleans missing and invalid values from the dataset

Separates:
--> Input features (X)
--> Target variable (portfolio_readiness_score)

Removes unnecessary columns such as:
--> Personal information
--> Contact details
--> URLs
--> Label columns
--> Internal evaluation metrics
--> Converts numerical fields into machine-readable format

Creates preprocessing pipelines for:
--> Numerical data
--> Categorical data

Performs:
--> Missing value imputation
--> Feature scaling
--> One-hot encoding

Generates cleaned feature datasets for machine learning models
Saves extracted structured features into a new CSV output file

Machine Learning Preprocessing Workflow:
--> Dataset loading
--> Missing value replacement
--> Feature-target separation
--> Data cleaning
--> Numerical conversion
--> Feature transformation
--> Encoding categorical variables
--> Saving processed output

Technologies & Libraries Used:
--> Python
--> Pandas
--> Scikit-learn
--> Pipeline API
--> ColumnTransformer
--> SimpleImputer
--> StandardScaler
--> OneHotEncoder

ML Concepts Implemented:
--> Feature Extraction
--> Data Cleaning
--> Feature Engineering
--> Data Transformation
--> Numerical Scaling
--> Categorical Encoding
--> Machine Learning Preprocessing Pipeline

Output Generated:
--> extracted_features_output.csv

Purpose:

This module prepares raw internship portfolio datasets into structured machine-learning-ready
feature matrices that can be directly used for:

--> ML model training
--> Benchmark testing
--> Resume readiness prediction
--> Internship scoring systems
--> Key Features:
--> Automated feature cleaning
--> Dynamic CSV loading
--> Structured preprocessing pipeline
--> Missing value handling
--> Numerical feature scaling
--> Categorical feature encoding
--> Exportable transformed dataset

************************************ train_pipeline.py ***************************************

This file is responsible for training the final Machine Learning regression model
for the Graphura Resume Readiness Score project.

Main Purpose:
The script trains a Random Forest Regressor model that predicts an intern's
portfolio/job readiness score based on extracted resume features.

Workflow of the File:
1. Reads the cleaned dataset from the processed data folder.
2. Imports preprocessing functions from extract_features.py.
3. Splits the dataset into training and testing sets.
4. Builds a preprocessing + ML pipeline.
5. Trains the Random Forest Regression model.
6. Evaluates model performance using RMSE and R² score.
7. Generates predicted readiness scores.
8. Scales scores into a 1–10 job readiness scale.
9. Saves:
   - trained model (.pkl)
   - scored dataset (.csv)

Important Libraries Used:
- pandas
- numpy
- scikit-learn
- joblib
- pathlib

Core ML Algorithm:
RandomForestRegressor

Evaluation Metrics:
- RMSE (Root Mean Squared Error)
- R² Score

Generated Outputs:
1. readiness_regression_model.pkl
   -> Saved trained ML model

2. intern_readiness_1_to_10_scores.csv
   -> Final intern ranking with predicted scores

Key Features:
- Automatic preprocessing pipeline
- Missing value handling
- Numerical feature scaling
- Categorical feature encoding
- Resume readiness prediction
- Intern ranking generation

Scoring Logic:
The model predicts portfolio readiness scores and converts them into
a normalized 1–10 scale for easier evaluation.

Example Output:
Intern Name                Predicted Score
------------------------------------------
Rahul Sharma                     9.2
Sneha Patil                      8.7
Amit Kumar                       7.9

Execution Command:
python train_model.py

Project Module Dependency:
This script depends on:
- extract_features.py

Author:
Graphura Resume Readiness Score Project (Team G)
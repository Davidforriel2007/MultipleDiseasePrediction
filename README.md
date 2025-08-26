# Multiple Disease Prediction System

## Project Name & Pitch

**Multiple Disease Prediction System**

A comprehensive machine learning web application that can predict three different diseases: Diabetes, Heart Disease, and Parkinson's Disease. Built with Streamlit, Python, and scikit-learn, this application demonstrates the practical application of machine learning in healthcare diagnostics through an intuitive web interface.

## Project Status

This project is complete and fully functional. Users can predict diabetes, heart disease, and Parkinson's disease by inputting relevant medical parameters. The application provides real-time predictions with clear success indicators.

## Installation and Setup Instructions

Clone down this repository. You will need `Python 3.7+` and `pip` installed globally on your machine.

Installation:

```bash
pip install -r requirements.txt
```

Or install packages individually:

```bash
pip install streamlit pandas numpy scikit-learn streamlit-option-menu
```

To Start Server:

```bash
streamlit run MultipleDisease.py
```

To Visit App:

`localhost:8501`

## Reflection

### What was the context for this project?
This was a machine learning project focused on healthcare diagnostics, built to demonstrate the practical application of ML models in disease prediction. The goal was to create a user-friendly interface for multiple disease prediction using trained machine learning models.

### What did you set out to build?
I set out to build a comprehensive disease prediction system that could:
- Predict diabetes using medical parameters like glucose levels, blood pressure, BMI, and other relevant factors
- Predict heart disease using cardiovascular health indicators including age, sex, chest pain types, blood pressure, cholesterol levels, and more
- Predict Parkinson's disease using voice analysis parameters (MDVP features) to detect early signs of the disease
- Provide an intuitive web interface for easy interaction with these prediction models

### Why was this project challenging and therefore a really good learning experience?
This project was challenging because it required:
- Integrating multiple pre-trained machine learning models into a single application
- Handling different data preprocessing requirements for each disease model
- Creating a user-friendly interface that could accommodate various input parameters
- Ensuring proper data validation and type conversion for user inputs
- Managing model persistence and loading in a production-like environment

### What were some unexpected obstacles?
- Standardizing input data (Normalization) across different disease prediction models
- Handling the feature scaling requirements for the Parkinson's disease model
- Creating an intuitive UI that could accommodate the different parameter sets for each disease
- Ensuring proper error handling for invalid user inputs

### What tools did you use to implement this project?

**Streamlit**: Chose Streamlit for the web interface because it provides rapid prototyping capabilities and excellent integration with Python data science libraries. It allowed for quick development of an interactive web application without the complexity of traditional web frameworks.

**Scikit-learn**: Used for the machine learning models and data preprocessing. The StandardScaler was particularly important for normalizing the Parkinson's disease features.

**Pandas & NumPy**: Essential for data manipulation and numerical operations. Pandas was used for reading the dataset and NumPy for array operations.

**Pickle**: Used for model persistence, allowing the trained models to be saved and loaded efficiently.

**Streamlit-option-menu**: Added for enhanced navigation between different disease prediction modules, providing a more professional user experience.

The choice of Streamlit over traditional web frameworks like Flask or Django was strategic - it allowed focus on the ML functionality rather than web development complexities, while still providing a professional user interface.

### Model Performance

The trained models achieved the following accuracy scores:
- **Diabetes Prediction Model**: 77% accuracy
- **Heart Disease Prediction Model**: 82% accuracy  
- **Parkinson's Disease Prediction Model**: 90% accuracy

These accuracy scores demonstrate the effectiveness of the machine learning models in predicting the respective diseases based on the input parameters.

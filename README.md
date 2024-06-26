# Health Care Center Application

The Health Care Center Application is a web-based tool that helps users identify diseases based on their symptoms and provides detailed information and recommendations. This project integrates various machine learning models to ensure accurate disease predictions and offers comprehensive health advice.


## Features

- Symptom-based disease prediction
- Detailed disease information including description, precautions, medications, workouts, and diets
- User-friendly interface with search functionality

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Flask
- **Machine Learning**: Scikit-learn
- **Data Handling**: Pandas
- **Model Persistence**: Pickle

## Setup and Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/JabedWeb/medicine-recommendation
    ```

2. **Create and activate a virtual environment:**
     ```sh
     python cd venv
     venv\Scripts\activate
     ```

3. **Run The flask Application**
    ```sh
    python app.py
    ```

4. **Open your browser and navigate to:**
    ```sh
    http://127.0.0.1:5000
    ```

## Project Structure

The project structure is as follows:

```
├── Datasets/
│   ├── description.csv
│   ├── diets.csv
│   ├── medications.csv
│   ├── precautions_df.csv
│   ├── workout_df.csv
│   └── symtoms_df.csv
├── Models/
│   └── svc.pkl
├── templates/
│   ├── index.html
│   ├── diseases.html
│   ├── diets.html
│   ├── about.html
│   ├── contact.html
│   └── blog.html
├── app.py
├── Recommendation_system.ipynb
└── README.md
```

## Data Collection

For the Health Care Center Application, we collected various datasets to provide accurate disease predictions and comprehensive health advice. Here are the details of the datasets used:

- **Workouts**: The `workout_df.csv` file contains a collection of workouts that are recommended for managing various health conditions. Each workout is associated with specific diseases and provides information on the type of exercise, duration, and intensity.

- **Descriptions**: The `description.csv` file includes detailed descriptions of different diseases. It provides information on the causes, symptoms, and effects of each disease, helping users understand the conditions better.

- **Precautions**: The `precautions_df.csv` file contains information on preventive measures for different diseases. It offers guidance on how to minimize the risk of contracting or spreading diseases.

- **Medications**: The `medications.csv` file includes a list of medications recommended for various diseases. It provides information on the dosage, frequency, and potential side effects of each medication.

- **Diets**: The `diets.csv` file provides diet recommendations for different health conditions. It includes information on the types of foods to consume or avoid to manage specific diseases.


## Model Training

Several machine learning models are trained to predict diseases based on symptoms:

- Support Vector Classifier (SVC)
- Random Forest
- Gradient Boosting
- K-Neighbors
- Multinomial Naive Bayes

These models are trained using the collected datasets and implemented in the `Recommendation_system.ipynb` notebook. Each model utilizes different algorithms and techniques to provide accurate disease predictions. The trained models are then saved in the `Models/` directory for future use.

To train the models, follow these steps:

1. Open the `Recommendation_system.ipynb` notebook.
2. Load the necessary datasets from the `Datasets/` directory.
3. Preprocess the data and extract relevant features.
4. Split the data into training and testing sets.
5. Initialize and train each machine learning model using the training data.
6. Evaluate the performance of each model using appropriate metrics.
7. Save the trained models in the `Models/` directory for future use.

By training multiple models, the Health Care Center Application ensures accurate disease predictions and provides users with reliable health advice.




# Salary Prediction Tool

This project provides a web-based Salary Prediction Tool using a machine learning model. Users can input their job details such as job title, years of experience, location, education level, company size, and relevant skills to get an estimated annual salary. The application also provides market insights like industry average, top 10% earners, growth potential, and demand level.

## Features

  * **Interactive Salary Prediction:** Users can input various professional details to receive a personalized salary estimate.
  * **User-Friendly Interface:** Built with Streamlit, offering an intuitive and responsive design.
  * **Market Insights:** Displays additional context like industry average salary, top earner potential, growth, and demand.
  * **Pre-trained Model:** Utilizes a pre-trained machine learning model (`best_salary_model.pkl`) for accurate predictions.
  * **Scalable and Customizable:** The underlying model and data can be updated for continuous improvement.

## Installation

To set up and run this project locally, follow these steps:

1.  **Clone the Repository:**

    ```bash
    git clone https://github.com/weakking140/salary_prediction2.git
    cd salary_prediction2
    ```

2.  **Create a Virtual Environment (Recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: `venv\Scripts\activate`
    ```

3.  **Install Dependencies:**
    All necessary libraries are listed in `requirements.txt`.

    ```bash
    pip install -r requirements.txt
    ```

## Usage

After installation, you can run the Streamlit application:

```bash
streamlit run app.py
```

This will open the application in your web browser, typically at `http://localhost:8501`.

## File Structure

The project directory contains the following key files:

  * `README.md`: Project description and setup instructions.
  * `app.py`: The main Streamlit application script.
  * `best_salary_model.pkl`: The trained machine learning model for salary prediction.
  * `label_encoders.pkl`: Stores label encoders used for transforming categorical features.
  * `skills_mlb.pkl`: Stores the MultiLabelBinarizer for encoding skills.
  * `final_salary_dataset.csv`: (Presumed) The dataset used for training the model.
  * `requirements.txt`: Lists all Python dependencies required to run the application.

## Technologies Used

  * **Streamlit:** For creating the interactive web application.
  * **Scikit-learn:** For machine learning functionalities, including model training and data preprocessing.
  * **Pandas:** For data manipulation and analysis.
  * **NumPy:** For numerical operations.
  * **joblib:** For saving and loading Python objects, particularly the machine learning model and encoders.
  * **XGBoost:** (Presumed, based on `requirements.txt`) Potentially used for the `best_salary_model.pkl`.

## Credits

This project was developed by weakking140.

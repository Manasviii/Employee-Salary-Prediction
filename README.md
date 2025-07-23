## 💰 Employee Salary Prediction App

A Streamlit web application to predict employee salaries based on experience, education, job title, company size, and location. Utilizes a Random Forest regression model trained on a synthetic dataset.

### Table of Contents
## Features

- Interactive salary prediction form
- Factors: Years of experience, education, job title, company size, location
- Detailed salary breakdown (base, experience, education, company, location)
- Model info and sample predictions displayed
- Streamlit interface with charts/metrics

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/salary-prediction-app.git
   cd salary-prediction-app
   ```

2. **Install requirements**
   ```bash
   pip install -r requirements.txt
   ```

3. **Generate sample data**
   ```bash
   python create_sample_data.py
   ```

4. **Train the model**
   ```bash
   python train_model.py
   ```

5. **Run the app**
   ```bash
   streamlit run app.py
   ```

## Usage

- Use the sidebar to input your details.
- Click "Predict Salary" to view results and breakdown.
- Optionally display sample predictions.

## Project Structure

| File                    | Description                             |
|-------------------------|-----------------------------------------|
| app.py                  | Streamlit app for prediction UI         |
| train_model.py          | Script to train & save the ML model     |
| create_sample_data.py   | Generates sample salary dataset         |
| requirements.txt        | Python dependencies                     |
| /data/salary_data.csv   | Generated dataset file                  |
| /models/salary_model.pkl| Trained ML model                        |

## Model Details

- Algorithm: Random Forest Regressor
- Features: 5 key attributes – experience, education, job title, company size, location
- Accuracy: R² > 0.85 (sample data)
- Data: 1,000+ synthetic records, realistic ranges and relationships

## Sample Predictions

| Years Experience | Education | Job Title         | Company Size | Location       | Predicted Salary |
|------------------|----------|-------------------|--------------|---------------|------------------|
| 2                | Bachelor | Software Engineer | Medium       | San Francisco | $104,299        |
| 10               | PhD      | Data Scientist    | Large        | New York      | $108,342        |
| ...              | ...      | ...               | ...          | ...           | ...              |



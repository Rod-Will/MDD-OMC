# MDD-OMC
Here is the updated `README.md` content tailored to your provided code and details:

```markdown
# AI Prediction for OMC and MDD

This repository contains the implementation of machine learning models to predict **Optimum Moisture Content (OMC)** and **Maximum Dry Density (MDD)**. These predictions are based on geotechnical soil properties using advanced regression techniques and hyperparameter optimization via **Particle Swarm Optimization (PSO)**. The project is released under the [CC0-1.0 License](LICENSE), making it publicly available for research and educational purposes.

---

## Features

- **Data Preprocessing:** Handles missing and non-numeric values to ensure clean data for training.
- **Advanced Models:** Implementation of:
  - Random Forest
  - Gradient Boosting
  - Support Vector Regression (SVR)
  - Neural Networks (MLPRegressor)
- **Hyperparameter Optimization:** Utilizes PSO to find optimal parameters for all models.
- **Model Evaluation:** Metrics include R² Score and Mean Squared Error (MSE) for performance comparison.
- **Visualization:** Heatmaps for correlation analysis and bar charts for performance metrics comparison.
- **Model Saving:** Best models are saved in `.pkl`, `.joblib`, or `.h5` formats for later use.

---

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Dataset](#dataset)
4. [Model Training](#model-training)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

---

## Installation

Clone the repository and install the necessary dependencies.

```bash
git clone https://github.com/yourusername/ai-prediction-omc-mdd.git
cd ai-prediction-omc-mdd
pip install -r requirements.txt
```

### Requirements

- Python 3.7+
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `keras`
  - `tensorflow`
  - `joblib`
  - `pyswarm`
  - `openpyxl`

Install all dependencies using the command:

```bash
pip install -r requirements.txt
```

---

## Usage

### Step 1: Prepare the Dataset

- Place your dataset (e.g., `MDD-OMC.xlsx`) in the `data/` folder.
- Ensure it includes the following columns:
  - `GC`, `SC`, `FC`, `LL`, `PL`, `PI`, `E` (features)
  - `OMC` (Optimum Moisture Content - target)
  - `MDD` (Maximum Dry Density - target)

### Step 2: Run the Script

Execute the main script to train and evaluate the models:

```bash
python main.py
```

### Step 3: Results and Models

- Results are visualized in the form of correlation heatmaps, prediction scatter plots, and performance bar charts.
- The best models are saved in the repository folder.

---

## Dataset

The dataset should include relevant soil properties as features and OMC/MDD as target variables. Example features:

- **GC:** Gravel Content
- **SC:** Sand Content
- **FC:** Fines Content
- **LL:** Liquid Limit
- **PL:** Plastic Limit
- **PI:** Plasticity Index
- **E:** Other engineering properties

A sample dataset (`MDD-OMC.xlsx`) is included for reference.

---

## Model Training

Hyperparameter optimization is performed using Particle Swarm Optimization (PSO). The following models are compared:

1. **Random Forest**
2. **Gradient Boosting**
3. **Support Vector Regression (SVR)**
4. **Neural Network (MLPRegressor)**

For each target variable (`OMC` and `MDD`):
- The dataset is split into training and testing sets (80:20 split).
- Models are trained using PSO to find the best hyperparameters.
- The best-performing model is saved.

---

## Results

### Visualization

- **Correlation Heatmap:** Displays relationships between features and target variables.
- **Prediction Scatter Plots:** Visualize predicted vs. actual values.
- **Bar Charts:** Compare R² and MSE scores for all models.

### Example Performance Metrics

| Model                 | R² (Train) | R² (Test) | MSE (Train) | MSE (Test) |
|-----------------------|------------|-----------|-------------|------------|
| Random Forest         | 0.90       | 0.88      | 0.012       | 0.015      |
| Gradient Boosting     | 0.89       | 0.87      | 0.014       | 0.018      |
| Support Vector Regression | 0.86   | 0.84      | 0.017       | 0.020      |
| Neural Network        | 0.92       | 0.89      | 0.010       | 0.014      |

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

---

## License

This project is licensed under the [CC0-1.0 License](LICENSE). Feel free to use, modify, and distribute the code without restriction.

---

## Acknowledgments

Special thanks to the geotechnical engineering and data science communities for their contributions to soil property research and machine learning innovations.

---

### Contact

For questions, feedback, or contributions, contact [rhudwill@gmail.com].
```

# Soil Compaction, MDD-OMC

```markdown
# Optimum Moisture Content (OMC) and Maximum Dry Density (MDD) Model Training  

This repository contains scripts, results, and visualizations for training machine learning models to predict **Optimum Moisture Content (OMC)** and **Maximum Dry Density (MDD)** using various algorithms. The workflow includes hyperparameter optimization, model evaluation, and visual representation of predictions.  

## Repository Structure  

```plaintext
├── data/                     # Dataset files used for training and testing  
├── notebooks/                # Jupyter Notebooks for exploratory analysis and experiments  
├── results/  
│   ├── plots/                # Plots from initial experiments and Grid prediction plots for optimized models 
│   ├── OMC_results.csv       # Model performance for OMC predictions  
│   ├── MDD_results.csv       # Model performance for MDD predictions  
├── scripts/                  # Python scripts for model training and evaluation  
├── README.md                 # Repository documentation  
```

## Models Trained  

### 1. **Optimum Moisture Content (OMC)**  
- **Models**:  
  - Random Forest  
  - Gradient Boosting (Best Performing Model)  
  - Support Vector Regression  
  - Neural Network  
- **Hyperparameter Optimization**:  
  - Performed using `RandomizedSearchCV` with predefined parameter spaces.  
- **Results**:  
  - Best model: **Gradient Boosting**  
  - Visualizations: Grid prediction plots saved in `results/plots2/`  

### 2. **Maximum Dry Density (MDD)**  
- **Models**:  
  - Random Forest  
  - Gradient Boosting (Best Performing Model)  
  - Support Vector Regression  
  - Neural Network  
- **Hyperparameter Optimization**:  
  - Similar to OMC, `RandomizedSearchCV` was used.  
- **Results**:  
  - Best model: **Gradient Boosting**  
  - Visualizations: Grid prediction plots saved in `results/plots2/`  

## Key Features  

- **Hyperparameter Optimization**: Optimized models using `RandomizedSearchCV` with warnings about parameter space constraints logged.  
- **Visualizations**: Grid prediction plots generated for each model and saved under `results/plots2/`.  
- **Model Evaluation**: Best-performing models identified for both OMC and MDD tasks.  

## Requirements  

The project uses Python and requires the following packages:  
- `scikit-learn`  
- `numpy`  
- `pandas`  
- `matplotlib`  
- `seaborn`  

Install dependencies using:  
```bash
pip install -r requirements.txt
```  

## Usage  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/OMC_MDD_Predictions.git
   cd OMC_MDD_Predictions
   ```  

2. Run the training scripts for OMC and MDD predictions:  
   ```bash
   python scripts/train_omc.py
   python scripts/train_mdd.py
   ```  

3. View results and visualizations in the `results/` directory.  

## Results  

- Best model for OMC: **Gradient Boosting**  
- Best model for MDD: **Gradient Boosting**  

## Future Work  

- Expand parameter spaces for hyperparameter optimization.  
- Integrate additional models like XGBoost and CatBoost.  
- Include feature importance analysis for better interpretability.  

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

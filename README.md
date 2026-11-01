# House Price Prediction using Data Science and Machine Learning

A beginner-friendly Data Science internship project that explores house-sales data, performs data cleaning and exploratory data analysis (EDA), trains a **Linear Regression** model, and evaluates house-price predictions.

## Project overview

- **Domain:** Data Science / Machine Learning
- **Language:** Python
- **Model:** Linear Regression
- **Notebook environment:** Google Colab or Jupyter Notebook
- **Dataset:** King County House Sales dataset

## Repository structure

```text
House_Price_Prediction_Project/
├── House_Price_Prediction.ipynb   # Complete project notebook
├── data/
│   └── .gitkeep                   # Keep this folder in GitHub; dataset is not included
├── outputs/
│   └── .gitkeep                   # Generated CSV results can be saved here
├── requirements.txt               # Python dependencies
├── .gitignore                     # Files not to commit
├── LICENSE                        # MIT License
└── README.md                      # Project documentation
```

## Dataset

Download the **King County House Sales** CSV dataset from Kaggle:

https://www.kaggle.com/datasets/harlfoxem/housesalesprediction

The notebook expects a CSV file containing a `price` column (the Kaggle file is commonly named `kc_house_data.csv`).

**Important:** The dataset is not included in this repository. Download it from Kaggle and upload it when the notebook asks for a CSV file. Do not upload private or restricted data.

## Run in Google Colab

1. Open the notebook file `House_Price_Prediction.ipynb` from this GitHub repository.
2. Click **Open in Colab** if available, or download the notebook and upload it at https://colab.research.google.com/.
3. Download the CSV dataset from the Kaggle link above.
4. Run the notebook cells from top to bottom.
5. When prompted, select the downloaded CSV file from your computer.
6. Review the EDA charts, model evaluation metrics, and sample prediction.
7. Download or commit the generated output files if you want to include them in your project report.

## Run locally (optional)

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd House_Price_Prediction_Project

python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
jupyter notebook House_Price_Prediction.ipynb
```

For local execution, place the dataset CSV in the project folder and adapt the notebook's Colab upload cell to read the local CSV, for example:

```python
df = pd.read_csv("data/kc_house_data.csv")
```

## Workflow

1. Import Python libraries (Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn).
2. Load and inspect the dataset.
3. Clean duplicate rows, missing values, and infinite values; remove identifier/date columns when present.
4. Perform EDA using distributions, scatter plots, box plots, and a correlation heatmap.
5. Select numeric input features and the `price` target.
6. Split the data into training and testing sets (80:20).
7. Train a Linear Regression model.
8. Generate predictions and evaluate them using:
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - R² score
9. Visualize actual vs. predicted prices and inspect model coefficients.
10. Export predictions and evaluation results to the `outputs/` folder.

## Results

Run the notebook to generate the actual evaluation metrics. **No accuracy or performance values are claimed in advance**, because results depend on the dataset and execution environment.

## Skills demonstrated

- Python programming
- Data cleaning and preprocessing
- Pandas and NumPy
- Exploratory Data Analysis
- Data visualization
- Scikit-learn
- Linear Regression
- Model evaluation

## Notes

- This is an educational project and its predictions should not be treated as professional property valuations.
- The dataset is provided by its original publisher; refer to the Kaggle dataset page for its terms and attribution.
- Replace `<YOUR_GITHUB_REPOSITORY_URL>` in the local setup command after creating your GitHub repository.

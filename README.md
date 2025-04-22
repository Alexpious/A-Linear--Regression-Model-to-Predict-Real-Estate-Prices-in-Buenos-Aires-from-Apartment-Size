
# 🏙️ A Regression Model to Predict Real Estate Prices in Buenos Aires from Apartment Size

This project applies a linear regression model to predict the price of apartments in **Buenos Aires** based on their **covered surface area** (in square meters). The goal is to understand the relationship between apartment size and price using real estate data, while also evaluating model performance using key metrics and visualizations.


## 📁 Dataset

The dataset used contains listings of real estate properties in Argentina. It was filtered down to only include:
- Properties located in **Capital Federal (Buenos Aires)**
- Property type: **Apartment**
- Price below **$400,000 USD**
- Surface area within the 10th to 90th percentile to remove outliers

---

## 📊 Visualizations

- **Scatter Plot** of apartment size vs. price  
- **Histogram** of apartment sizes  
- **Regression Line** plotted against training and test sets  

These visualizations help to understand the relationship between size and price, and to assess the model fit visually.

---

## 🧠 Model

A **Linear Regression** model was trained with:
- **Features:** `surface_covered_in_m2`  
- **Target:** `price_aprox_usd`

**Steps taken:**
1. Data wrangling and filtering
2. Train-test split (80/20)
3. Baseline model using mean price
4. Training the linear model
5. Evaluating model using **Mean Absolute Error (MAE)**
6. Plotting predicted vs actual values
7. Extracting model coefficients

---

## 📈 Results

- **Baseline MAE:** Computed using the mean of `y_train`
- **Training MAE:** MAE from predictions on training data
- **Test MAE:** Final evaluation on unseen data
- **Regression Equation:**  
  `Predicted Price = intercept + coefficient * surface_covered_in_m2`


## 🛠️ Tech Stack

- **Python**
- **Pandas**
- **Matplotlib**
- **Scikit-learn**

---

## 🚀 Getting Started

1. Clone the repository  
   ```bash
   git clone https://github.com/your-username/buenos-aires-real-estate-prediction.git
   cd buenos-aires-real-estate-prediction
   ```
2. Install dependencies  
   ```bash
   pip install pandas matplotlib scikit-learn
   ```
3. Run the script  
   ```bash
   python real_estate_model.py
   ```


Let me know if you want a version with markdown badges, or if you want help writing the `requirements.txt` or pushing to GitHub.

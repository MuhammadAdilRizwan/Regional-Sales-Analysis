# Regional Sales Analysis

A Python-based data analysis and machine learning project that explores **Adidas US Sales** data across regions, states, and cities. The project was developed as a PAI (Python for Artificial Intelligence) course project.

---

## 📁 Repository Structure

```
Regional-Sales-Analysis/
├── Adidas US Sales Datasets.csv   # Source dataset (~9,648 records)
├── PAI_Project.ipynb              # Initial project notebook
└── PAI_Project_Final.ipynb        # Final project notebook
```

---

## 📊 Dataset

**File:** `Adidas US Sales Datasets.csv`

The dataset contains Adidas retail sales records across the United States with the following columns:

| Column | Description |
|---|---|
| `Retailer` | Name of the retailer (e.g., Foot Locker, Amazon) |
| `Retailer ID` | Unique identifier for each retailer |
| `Invoice Date` | Date of the sale |
| `Region` | US region (Northeast, Southeast, Midwest, South, West) |
| `State` | US state |
| `City` | City of sale |
| `Product` | Product category (e.g., Men's Street Footwear) |
| `Price per Unit` | Selling price per unit |
| `Units Sold` | Number of units sold |
| `Total Sales` | Total revenue generated |
| `Operating Profit` | Profit from operations |
| `Operating Margin` | Operating profit as a percentage of sales |
| `Sales Method` | Channel used (In-store, Online, Outlet) |

---

## 🔍 Analysis Performed

### Exploratory Data Analysis
- Unique products, retailers, states, regions, cities, and sales methods
- Total units sold per state and per city
- Average units sold per city and per state
- Pandas operations demonstrated: `columns`, `index`, `head`, `tail`, `info`, `describe`, `iloc`, `concat`, `Series`
- Boolean filtering (e.g., units sold > 1000, filtered by product)
- Statistical functions: `mean`, `max`, `between`

### Visualizations
- **Bar Chart** – Unit sales across US cities
- **Pie Chart** – Total sales distribution by region
- **Pie Chart** – Units sold distribution by region
- **Pie Chart** – Best sales method (In-store / Online / Outlet)
- **Bar Chart** – Total sales by retailer
- **Bar Chart** – Operating profit by product

### Machine Learning
| Model | Features | Target |
|---|---|---|
| Linear Regression | Units Sold | Total Sales |
| Decision Tree Classifier | Total Sales | Operating Profit |
| Naive Bayes (GaussianNB) | Total Sales | Operating Profit |

---

## 🛠️ Technologies Used

- **Python 3**
- **Jupyter Notebook**
- **pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Matplotlib** – Data visualization
- **scikit-learn** – Machine learning models and evaluation
- **SciPy** – Statistical analysis (linear regression)

---

## 🚀 Getting Started

### Prerequisites

Install the required Python packages:

```bash
pip install pandas numpy matplotlib scikit-learn scipy jupyter
```

### Running the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/MuhammadAdilRizwan/Regional-Sales-Analysis.git
   cd Regional-Sales-Analysis
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open `PAI_Project_Final.ipynb` and update the CSV file path in the first cell to point to your local copy of `Adidas US Sales Datasets.csv`:
   ```python
   dataframe = pd.read_csv('Adidas US Sales Datasets.csv', skiprows=3)
   ```

4. Run all cells (Kernel → Restart & Run All).

---

## 👥 Authors

- **22k-4018**
- **22k-4082**
- **22k-4059**

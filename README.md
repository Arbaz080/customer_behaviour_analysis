# Customer Shopping Behavior Analysis

## 📋 Project Overview

This project analyzes customer shopping behavior patterns using a comprehensive dataset of 3,900 customer transactions. The analysis combines Python for data cleaning and exploration, PostgreSQL for advanced querying, and Power BI for interactive visualization. The goal is to uncover actionable insights about customer demographics, purchasing patterns, and subscription behaviors to drive data-driven business decisions.

## 📊 Dataset

**Source:** Customer Shopping Behavior Dataset  
**Records:** 3,900 transactions  
**Features:** 18 columns including:
- Customer demographics (Age, Gender, Location)
- Purchase details (Item, Category, Amount, Season)
- Product attributes (Size, Color, Review Rating)
- Customer behavior (Previous Purchases, Frequency, Subscription Status)
- Transaction details (Shipping Type, Discount Applied, Payment Method)

**Key Data Cleaning Steps:**
- Handled 37 missing values in Review Rating using category-wise median imputation
- Created age groups (Young Adult, Adult, Middle-aged, Senior) for demographic analysis
- Converted purchase frequency to numerical days for comparison
- Removed redundant column (promo_code_used) as it duplicated discount_applied

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python** | Data cleaning, transformation, and EDA |
| **Pandas** | Data manipulation and analysis |
| **PostgreSQL** | Database management and advanced SQL queries |
| **Power BI** | Interactive dashboard creation and visualization |
| **Jupyter Notebook** | Code development and documentation |
| **Gamma** | Professional presentation creation |

## 🔄 Project Workflow

### 1. Data Preparation (Python)
- Loaded CSV data using Pandas
- Performed exploratory data analysis (EDA)
- Handled missing values with category-based imputation
- Created derived columns (age_group, purchase_frequency_days)
- Standardized column names for SQL compatibility
- Exported cleaned data to PostgreSQL

### 2. Database Analysis (PostgreSQL)
Executed 10 analytical SQL queries including:
- Revenue analysis by gender and age group
- Top-rated products identification
- Discount impact assessment
- Customer segmentation (New, Returning, Loyal)
- Subscription vs. spending correlation
- Shipping type comparison
- Category-wise product performance

### 3. Visualization (Power BI)
Built an interactive dashboard featuring:
- Revenue distribution by demographics
- Product category performance
- Customer segmentation analysis
- Subscription impact on revenue
- Geographic sales patterns
- Review ratings and product popularity

### 4. Reporting
- Compiled comprehensive analysis report
- Created executive presentation using Gamma
- Documented key findings and recommendations

## 📈 Key Insights

1. **Gender Revenue Split:** Analysis of revenue contribution by gender
2. **High-Value Discount Users:** Customers using discounts who still exceed average purchase amounts
3. **Top-Rated Products:** Products with highest average review ratings
4. **Subscription Value:** Subscribers show higher average spending and total revenue
5. **Customer Loyalty:** 3-tier segmentation reveals distinct spending patterns
6. **Seasonal Trends:** Purchase patterns vary by season and category
7. **Shipping Preferences:** Comparison of Express vs. Standard shipping spend

## 🎯 Dashboard Features

The Power BI dashboard includes:
- **Overview Page:** Key metrics and revenue trends
- **Customer Analysis:** Demographics and segmentation
- **Product Performance:** Category and item-level insights
- **Geographic Distribution:** Location-based sales patterns
- **Interactive Filters:** Dynamic filtering by age group, category, season, and more

## 💻 How to Run This Project

### Prerequisites
```bash
Python 3.8+
PostgreSQL 12+
Power BI Desktop
Jupyter Notebook
```

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/customer-behavior-analysis.git
cd customer-behavior-analysis
```

### Step 2: Install Python Dependencies
```bash
pip install pandas sqlalchemy psycopg2-binary
```

### Step 3: Set Up PostgreSQL Database
```sql
CREATE DATABASE customer_behaviour;
```

### Step 4: Run the Jupyter Notebook
```bash
jupyter notebook Customer_Shopping_Behaviour_Analysis.ipynb
```
- Execute all cells to clean data and load into PostgreSQL
- Update database credentials in the notebook (username, password, host)

### Step 5: Execute SQL Queries
- Open PostgreSQL (pgAdmin or command line)
- Run queries from `customer_behavior_sql_queries.sql`
- Analyze query results

### Step 6: Open Power BI Dashboard
- Open `customer_behaviour_dashboard.pbix` in Power BI Desktop
- Update data source connection if needed
- Explore interactive visualizations

## 📁 Project Structure

```
customer-behavior-analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── Customer_Shopping_Behaviour_Analysis.ipynb
│
├── sql/
│   └── customer_behavior_sql_queries.sql
│
├── dashboards/
│   └── customer_behaviour_dashboard.pbix
│
├── reports/
│   ├── analysis_report.pdf
│   └── presentation.pdf
│
└── README.md
```

## 🎓 Learning Outcomes

- End-to-end data analytics workflow
- Data cleaning and transformation with Python
- Database integration with SQLAlchemy
- Complex SQL query writing
- Interactive dashboard design
- Business insights generation
- Professional reporting and presentation

## 👤 Author

**Arbaz Khan**  
- LinkedIn: [your-profile](https://www.linkedin.com/in/arbaz-khan-8b114621a/)
- GitHub: [your-username](https://github.com/Arbaz080)
- Email: arbazkhan0804@gmail.com

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Dataset source: 'customer_shopping_behavior.csv'
- Tools and libraries used in this analysis
- Community resources and documentation

---

⭐ If you found this project helpful, please consider giving it a star!

**Last Updated:** October 2025

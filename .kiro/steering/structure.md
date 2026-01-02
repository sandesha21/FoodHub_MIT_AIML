# Project Structure

## Repository Organization

```
foodhub-analysis/
├── .git/                           # Git version control
├── .gitignore                      # Git ignore patterns
├── .kiro/                          # Kiro AI assistant configuration
│   └── steering/                   # AI guidance documents
├── .vscode/                        # VS Code workspace settings
├── LICENSE                         # Project license
├── README.md                       # Project documentation
├── foodhub_order.csv              # Primary dataset (1,898 orders)
└── Project1_Foodhub_sbadwaik_Learner_Notebook_Full_Code_Submission.ipynb
```

## File Conventions

### Data Files
- **Primary Dataset**: `foodhub_order.csv`
  - Contains 1,898 rows × 9 columns
  - Clean dataset with no missing values
  - Includes order details, restaurant info, delivery metrics

### Notebook Structure
- **Main Analysis**: Single comprehensive Jupyter notebook
- **Naming Convention**: Descriptive filename with author identifier
- **Content Organization**:
  - Data loading and preprocessing
  - Exploratory Data Analysis (EDA)
  - Statistical analysis and insights
  - Visualizations and business recommendations

## Data Schema

### Core Entities
- **Orders**: Unique transactions with order_id as primary key
- **Customers**: 1,200 unique customers identified by customer_id
- **Restaurants**: 178 unique restaurants with restaurant_name
- **Cuisines**: 14 different cuisine types

### Key Relationships
- One-to-many: Customer → Orders
- One-to-many: Restaurant → Orders
- One-to-many: Cuisine Type → Orders

## Development Workflow
1. **Data Loading**: Import CSV using pandas
2. **Data Cleaning**: Type optimization and validation
3. **Exploratory Analysis**: Univariate, bivariate, and multivariate analysis
4. **Visualization**: Charts and plots for insights
5. **Business Insights**: Actionable recommendations

## File Naming Standards
- Use descriptive, lowercase filenames
- Separate words with underscores
- Include version or author info for notebooks
- Keep data files in root directory for easy access
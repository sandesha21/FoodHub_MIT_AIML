# Technology Stack

## Programming Language & Environment
- **Primary Language**: Python 3.13+
- **Development Environment**: Jupyter Notebook / Google Colab
- **Data Format**: CSV files

## Core Libraries & Dependencies
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing and array operations
- **matplotlib**: Data visualization and plotting
- **seaborn**: Statistical data visualization

## Data Processing Approach
- **Data Types**: Mixed (integers, floats, categorical data, objects)
- **Memory Optimization**: Uses pandas categorical data types for efficiency
- **Missing Values**: Dataset is clean with no missing values

## Common Commands & Workflows

### Environment Setup
```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

### Data Loading
```python
df = pd.read_csv('foodhub_order.csv')
```

### Data Type Optimization
```python
df['day_of_the_week'] = df['day_of_the_week'].astype('category')
df['cuisine_type'] = df['cuisine_type'].astype('category')
df['customer_id'] = df['customer_id'].astype('category')
df['restaurant_name'] = df['restaurant_name'].astype('category')
```

### Basic Analysis Commands
```python
# Dataset overview
df.info()
df.shape
df.head()

# Statistical summary
df.describe()

# Missing values check
df.isna().sum()

# Unique value counts
df['column_name'].value_counts()
df['column_name'].nunique()
```

## Development Standards
- Use descriptive variable names
- Optimize memory usage with appropriate data types
- Include observations and insights after each analysis step
- Follow exploratory data analysis (EDA) workflow: univariate → bivariate → multivariate analysis
## Data Normalization, Exploration, and Preparation


## Example: Python Code for Prediction

### Normalizing the Ecommerce Dataset


Below is the Python code for creating a normalized SQLite database, inserting data into relational tables, and processing the dataset.

```{code-cell} python
import sqlite3
import pandas as pd
import warnings
warnings.filterwarnings("ignore")

# Load the dataset
df = pd.read_csv("/Users/ramprakashyallavula/Downloads/ecommerce project/Ecommerce_Sales_Prediction_Dataset.csv")

# Connect to SQLite database (it will create the database file if it doesn't exist)
conn = sqlite3.connect('/Users/ramprakashyallavula/Downloads/ecommerce_sales.db')
cursor = conn.cursor()

# Create tables and insert data (shortened for brevity)
cursor.execute("""
    CREATE TABLE IF NOT EXISTS Products (
        ProductID INTEGER PRIMARY KEY AUTOINCREMENT,
        ProductCategory TEXT,
        Price REAL,
        Discount REAL
    );
""")
# Additional code
conn.close()
print("Normalized database created and data inserted successfully.")
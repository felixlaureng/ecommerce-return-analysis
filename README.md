# E-Commerce Return Analysis

An e-commerce analytics project investigating product return patterns, delivery performance, and transactional factors using SQL, Python, PostgreSQL on Neon, and Tableau.

## Project Overview

Product returns can affect revenue, customer satisfaction, and operational efficiency in e-commerce. This project explores transaction data to identify patterns associated with returns and investigate potential relationships between return behavior, product price segments, delivery performance, and geographic factors.

## Business Objectives

- Analyze transaction and return patterns across relevant segments.
- Investigate return behavior across product price segments.
- Examine the relationship between delivery performance and returns.
- Explore geographic differences in return patterns.
- Translate analytical findings into actionable business recommendations.

## Tech Stack

- **Neon** — Managed serverless PostgreSQL database.
- **PostgreSQL & SQL** — Data querying, extraction, and aggregation.
- **Python & Pandas** — Data processing, cleaning, and exploratory analysis.
- **SQLAlchemy** — Database connectivity.
- **Tableau** — Data visualization and dashboard development.

## Analytical Workflow

### 1. Data Extraction

Query transaction and order data stored in Neon PostgreSQL using SQL.

### 2. Data Preparation

Clean and transform the extracted data using Python and Pandas. Prepare analytical variables such as price segments, shipping duration, geographic attributes, and return indicators, where supported by the source data.

### 3. Exploratory Data Analysis

Explore transaction and return patterns across product price segments, delivery performance, and geographic dimensions.

### 4. Statistical Analysis

Evaluate relationships between return behavior and selected transactional or operational variables. Interpret results based on the available data and analytical assumptions.

### 5. Visualization & Recommendations

Present the results through Tableau visualizations and develop business recommendations supported by the analysis.

## Key Findings

- **Return patterns:** Document the main patterns found in the dataset.
- **Price segments:** Summarize differences in return behavior across price categories, if observed.
- **Delivery performance:** Report the observed relationship between shipping duration and returns.
- **Geographic analysis:** Highlight meaningful regional differences, where supported by the data.

## Getting Started

### Prerequisites

- Python 3.9 or a compatible environment.
- A Neon PostgreSQL database with the required tables.
- Tableau Desktop or Tableau Reader, if needed to inspect the workbook.

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/ecommerce-return-analysis.git
cd ecommerce-return-analysis
```

### 2. Create a Virtual Environment

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### 3. Configure the Database Connection
This project uses a PostgreSQL database hosted on Neon.
Create a `.env` file in the project root and configure your Neon PostgreSQL connection string:

```env
DATABASE_URL=your_neon_postgresql_connection_string
```
Load the environment variable in Python and connect to the database using psycopg2:

import os
import psycopg2
from dotenv import load_dotenv

load_dotenv()

conn = psycopg2.connect(os.environ["DATABASE_URL"])

Ensure that .env is included in .gitignore to prevent credentials from being committed to GitHub.

### 4. Run the Analysis

Ensure the required dataset and database tables are available, then execute the SQL queries and run the analysis notebook.
Detailed setup instructions may be added as needed to reproduce the analysis.

## Limitations

- Results depend on source data completeness and quality.
- Observed relationships do not necessarily establish causation.
- Return definitions must match the fields available in the dataset.
- Findings may not generalize to other e-commerce platforms or time periods.

## Future Improvements

- Automate data extraction and transformation.
- Add data quality checks and validation.
- Develop a repeatable analytics pipeline.
- Expand dashboard metrics and monitoring.

## Author

**Felix Ferdinand Laureng**

Data Analytics | SQL | Python | Business Intelligence

[LinkedIn]((https://www.linkedin.com/in/felix-ferdinand-laureng/)) · [GitHub](https://github.com/felixlaureng)

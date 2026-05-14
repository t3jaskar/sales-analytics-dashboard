# Sales Analytics Dashboard

An end-to-end data engineering and analytics project built using Python, PostgreSQL, dbt, Pandas, Plotly Dash, Docker, and Great Expectations.

This project uses the Brazilian E-Commerce (Olist) dataset to build a scalable analytics pipeline with data validation, warehouse modeling, and interactive dashboards.

---

## Features

- ETL pipeline using Python and Pandas
- PostgreSQL data warehouse
- dbt transformations with staging, fact, and dimension models
- Slowly Changing Dimension (SCD Type 2) implementation
- Data validation using Great Expectations
- Interactive dashboard with Plotly Dash
- Dockerized setup for portability
- Environment variable management using `.env`

---

## Tech Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Database | PostgreSQL |
| Data Transformation | dbt |
| Data Processing | Pandas |
| Visualization | Plotly Dash |
| Data Validation | Great Expectations |
| Containerization | Docker |
| Version Control | Git & GitHub |

---

## Project Structure

```bash
sales-analytics-dashboard/
│
├── data/
├── notebooks/
├── scripts/
├── dashboard/
├── dbt_project/
├── great_expectations/
├── docker/
├── .env
├── requirements.txt
├── docker-compose.yml
├── README.md
└── .gitignore
```

---

## Setup Instructions

### 1. Clone Repository

```bash
git clone <your-repo-url>
cd sales-analytics-dashboard
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

### 3. Activate Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### Mac/Linux

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## PostgreSQL Setup

Create a PostgreSQL database:

```sql
CREATE DATABASE sales_analytics;
```

Update your `.env` file:

```env
DB_HOST=localhost
DB_PORT=5432
DB_NAME=sales_analytics
DB_USER=postgres
DB_PASSWORD=your_password
```

---

## Run ETL Pipeline

```bash
python scripts/load_data.py
```

---

## Run dbt Models

```bash
dbt run
```

---

## Run Great Expectations Validation

```bash
great_expectations checkpoint run sales_checkpoint
```

---

## Run Dashboard

```bash
python dashboard/app.py
```

---

## Future Improvements

- Kafka-based streaming pipeline
- Redis caching layer
- Airflow orchestration
- CI/CD pipeline
- Cloud deployment (AWS/GCP/Azure)
- Advanced forecasting models

---

## Dataset

Brazilian E-Commerce Public Dataset by Olist.

---

## Author

Tejaskar Mahanta

Backend Developer | Data Engineering Enthusiast
# Airflow DAGs Repository

Welcome to the central repository for our team's Airflow DAGs. This project contains the orchestration logic for various data pipelines, analytics jobs, and operational workflows. The goal is to maintain a clean, organized, and collaborative space for all our automated tasks.

---

## Getting Started

To add or modify a DAG, please follow these general guidelines:

1. **Create Your Own Folder**  
   Name it `transformation_to_(parquet|iceberg|deltalake)/` if it doesn’t already exist in the repo.

2. **Add Your DAGs**  
   Place your Python DAG files inside your project folder.

3. **Document Your Work**  
   Add an entry for each of your primary DAGs in the **DAGs Catalog** section below.

4. **Commit and Push**  
   Use clear and descriptive commit messages to explain your changes.

---

## DAGs Catalog

This catalog provides a quick overview of available DAGs, their purpose, and maintainers. Please add an entry for your DAGs following the template below.

### Data Lake Transformation Pipeline

- **Pipeline:** `CSV to Delta Lake Transformation`  
- **Maintainer:** Lavanya Kalla  
- **Description:** Ingests raw CSV data from various sources, validates its structure, cleanses and transforms it, and loads it into a partitioned Delta Lake table for analytics.  
- **DAGs:**  
  - `schema_validation_dag` — Validates the schema (column names and data types) of source CSV files to ensure structural integrity before processing.

---

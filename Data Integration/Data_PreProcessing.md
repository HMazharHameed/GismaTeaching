# Data Cleaning and Preprocessing in Spark SQL

## Scenario

You are working as a data engineer for a startup that collects customer feedback from multiple sources. You have been handed a messy dataset exported from their internal feedback system.

Your goal is to clean and prepare this dataset so that the analytics team can build dashboards and sentiment analysis models.

---

## Dataset Description

The dataset contains the following issues:

- Missing values in key fields (e.g., `customer_id`, `feedback_text`, `rating`)
- Inconsistent capitalization and extra spaces in text fields
- Ratings stored as strings instead of integers
- Some feedback entries are duplicated
- Placeholder values like `"N/A"` or `"null"` appear as text
- Several records are missing the `submitted_at` timestamp or contain invalid date formats

---

## Your Tasks

### Step 1: Load and Inspect

- Load the CSV or JSON dataset into a DataFrame.
- Print schema, null value counts, and sample entries.

---

### Step 2: Clean and Transform

- Replace placeholder text values (`"N/A"`, `"null"`, `"unknown"`) with `null`.
- Use `.na.drop()` or `.na.fill()` where appropriate.
- Trim and standardize the `feedback_text` column (remove whitespace, convert to lowercase).
- Convert `rating` column to integer and handle invalid ratings (e.g., outside 1–5 range).
- Parse and standardize the `submitted_at` column into proper date format using Spark functions.

---

### Step 3: Deduplicate

- Drop duplicates based on a subset of fields: `customer_id`, `feedback_text`, and `submitted_at`.

---

### Step 4: Save and Review

- Save the cleaned DataFrame as a CSV file.
- Reload and show 10 cleaned entries for verification.



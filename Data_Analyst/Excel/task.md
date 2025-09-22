# 🧹 Data Cleaning Assignment

## Dataset

📂 Use the file: `sales_dataset_messy.xlsx` (or CSV version).

---

## Tasks

### 1. Handling Missing Data

* Identify how many missing values are present in each column.
* Decide and justify: Should you remove or fill missing values?
* Example: Fill missing `Customer Name` with "Unknown".

---

### 2. Removing Extra Spaces

* Detect and clean unnecessary leading/trailing spaces in `Customer Name` and `City`.
* Example: " John Doe " → "John Doe".

---

### 3. Handling Duplicates

* Check for duplicate rows.
* Remove duplicates and mention how many were removed.

---

### 4. Standardizing Data

* Ensure `State` names are consistent (e.g., "Maharashtra " → "Maharashtra").
* Convert all `Product Category` values to Title Case (e.g., "electronics" → "Electronics").

---

### 5. Checking Data Types

* Make sure:

  * `Sale Date` → Date format
  * `Quantity` → Integer
  * `Price per unit` & `Sales Amount` → Numeric (float)

---

### 6. Validating Calculations

* Verify that:

  * `Sales Amount = Quantity × Price per unit`
* If mismatches are found, correct them.

---

### 7. Export Clean Data

* Save the cleaned dataset as:

  * `sales_dataset_cleaned.xlsx`
  * `sales_dataset_cleaned.csv`

---

## Submission

* Submit the cleaned file + a short report (in Word/PDF) describing what changes were made and why.

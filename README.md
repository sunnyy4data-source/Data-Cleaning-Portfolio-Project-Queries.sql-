🧹 Nashville Housing Data Cleaning with SQL

📌 Project Overview
This project demonstrates a complete SQL-based data cleaning pipeline applied to a real-world housing dataset from Nashville, Tennessee. The goal is to transform raw, inconsistent property records into a clean, structured format ready for analysis, simulation modeling, and dashboarding.

🛠️ Key Cleaning Steps
1. Date Standardization
Converted SaleDate into SQL-native Date format for accurate filtering and time-based analysis.

2. Missing Address Imputation
Filled null PropertyAddress values by matching ParcelID across duplicate entries using self-joins.

3. Address Parsing
Split both PropertyAddress and OwnerAddress into separate columns (Street, City, State) using SUBSTRING and PARSENAME.

4. Categorical Normalization
Standardized SoldAsVacant field from 'Y'/'N' to 'Yes'/'No' using CASE statements for clarity.

5. Duplicate Removal
Used ROW_NUMBER() with PARTITION BY to identify and remove duplicate rows based on key fields.

6. Column Optimization
Dropped irrelevant columns like OwnerAddress, TaxDistrict, and raw PropertyAddress to streamline the dataset.

📂 Technologies Used
Microsoft SQL Server

SQL Server Management Studio (SSMS)

T-SQL (Transact-SQL)

📈 Use Cases
Clean dataset for simulation modeling (e.g., airport security flows)

Ready for dashboard creation in Excel or Power BI

Ideal for statistical analysis using Minitab or Python (Pandas)

📥 Data Import Options
Includes setup for advanced import using OPENROWSET and BULK INSERT (requires server configuration).

✅ Status
✔️ Data cleaned and transformed ✔️ Ready for analysis and visualization ✔️ Modular SQL scripts for reuse

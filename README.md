# Nashville Housing Data Cleaning Project

## Overview
This project focuses on cleaning and standardizing the Nashville Housing dataset. The SQL queries address issues such as standardizing date formats, populating missing property addresses, breaking down addresses into individual columns, and normalizing 'SoldAsVacant' values. The cleaning process involves handling duplicates and removing unused columns for a more refined dataset.

## Project Structure

### 1. Standardize Date Format
- Converts the 'SaleDate' column to a standardized date format.

### 2. Populate Property Address Data
- Populates missing property addresses by updating null values based on ParcelID.

### 3. Break Out Property Address into Individual Columns
- Splits the 'PropertyAddress' column into 'PropertySplitAddress' and 'PropertySplitCity'.

### 4. Break Out Owner Address into Individual Columns
- Uses `parsename` to split 'OwnerAddress' into 'OwnerSplitAddress', 'OwnerSplitCity', and 'OwnerSplitState'.

### 5. Change 'Y' and 'N' to 'Yes' and 'No' in 'SoldAsVacant' Field
- Updates the 'SoldAsVacant' column to replace 'Y' with 'Yes' and 'N' with 'No'.

### 6. Remove Duplicates
- Identifies and displays duplicate records based on specific columns.

### 7. Delete Unused Columns
- Drops columns 'OwnerAddress', 'TaxDistrict', 'PropertyAddress', and 'SaleDate' to streamline the dataset.

## Usage
1. Clone the repository: `git clone https://github.com/SaiSurajMatta/Nashville-Housing-Data-Cleaning-Project`
2. Execute the SQL queries in the specified order on your SQL environment.
3. Explore the cleaned Nashville Housing dataset with refined structure and standardized values.

Feel free to contribute, suggest improvements, or adapt the queries for similar data-cleaning tasks.

## Dataset
Dataset Link: https://www.kaggle.com/datasets/tmthyjames/nashville-housing-data
- The project utilizes the Nashville Housing dataset.

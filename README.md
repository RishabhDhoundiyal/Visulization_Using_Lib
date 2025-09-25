# Netflix Titles Data Cleaning, Preprocessing and Visualization
Cleaned Netflix data by handling missing values (filled director/cast/country, dropped rows for date/rating/duration), removed duplicates, standardized text (stripped spaces, lowercased except titles), converted 'date_added' to datetime, and ensured correct data types like integer 'release_year'.


# Data Cleaning Steps  
This section outlines the steps taken to clean and preprocess the Netflix Titles dataset.

- 1.Loading the Data: The dataset was loaded into a pandas DataFrame from the netflix_titles.csv file.
- 2.Handling Missing Values:
   - Missing values in the 'director', 'cast', and 'country' columns were filled with the string 'Unknown'.
   - Rows with missing values in the 'date_added' or 'rating' columns were removed.
   - Rows with missing values in the 'duration' column were removed.
- 3.Removing Duplicates: Exact duplicate rows in the dataset were identified and removed.
- 4.Standardizing Text Data:
   - Leading and trailing whitespace was removed from text columns ('type', 'title', 'director', 'cast', 'country', 'rating', 'duration', 'listed_in', 'description').
   - Text in these columns (except 'title') was converted to lowercase for consistency.
   - The 'title' column was converted to title case.
- 5.Converting Date Format: The 'date_added' column was converted to a datetime object to ensure consistent date handling. Any values that could not be parsed were converted to NaT (Not a Time).
- 6.Renaming Columns: Column headers were checked and confirmed to be in a clean and uniform format.
- 7.Checking and Fixing Data Types: The 'release_year' column was converted to an integer data type.


# Author
[Rishabh Dhoundiyal](https://github.com/RishabhDhoundiyal)

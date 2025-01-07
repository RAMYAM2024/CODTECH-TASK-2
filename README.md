Data Analysis with PySpark

This project demonstrates the use of PySpark for basic data analysis tasks, including filtering, grouping, and aggregating data. The results are saved to a CSV file for further use.

Features

- **Filter Data**: Select rows based on specified conditions.
- **Group and Aggregate**: Perform group-by operations and calculate summary statistics (e.g., average age and count).
- **Save Results**: Export the processed data to a CSV file.

Prerequisites

- Python 3.x
- Apache Spark (PySpark)

Installation

1. Install PySpark:
   ```bash
   pip install pyspark
   ```

2. Verify the installation:
   ```bash
   pyspark --version
   ```

Usage

1. Clone this repository or copy the script.
2. Replace the `path/to/analysis_results.csv` with your desired output file path.
3. Run the script:
   ```bash
   python script_name.py
   ```

Script Overview

Sample Dataset
The script uses a sample dataset representing individuals with their IDs, names, ages, and occupations:

| ID  | Name       | Age | Occupation |
|-----|------------|-----|------------|
| 1   | Anna       | 25  | Engineer   |
| 2   | Brian      | 30  | Doctor     |
| 3   | Catherine  | 35  | Lawyer     |
| 4   | Daniel     | 40  | Engineer   |
| 5   | Ella       | 50  | Scientist  |

Steps

1. **Initialize Spark Session**: Create a Spark session for data processing.
2. **Load Data**: Use a sample dataset defined in the script.
3. **Filter Rows**: Select rows where age is greater than 25.
4. **Group and Aggregate**: Calculate the average age and count of individuals in each occupation group.
5. **Save Results**: Save the aggregated results to a CSV file.

Output

The script generates a CSV file with the following structure:

| Occupation | Average_Age | Count |
|------------|-------------|-------|
| Doctor     | 30.0        | 1     |
| Engineer   | 35.0        | 2     |
| Lawyer     | 35.0        | 1     |
| Scientist  | 50.0        | 1     |

License

This project is licensed under the MIT License. Feel free to use, modify, and share.



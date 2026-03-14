Data Preprocessing And Cleaning On  (Jupiter Notebook)

Steps Involved In Cleaning Of A Messy Dataset ,Environment Used Here Is Kaggle Notebook

1 Importing Essentials Lib
First of all, we need to import certain lib which are dedicated for such task in data analytics. The crucial part of any analysis is that the dataset of which we are going to work should be free form any redundacy, so these lib python which works on top of it helps in cleaning of data which contains thousands and millions of row.

NumPy (Numerical Python), Pandas (Python Data Analysis), and Matplotlib are foundational Python libraries in data analysis, each serving a distinct but complementary role in the workflow, NumPy provides the core functionality for efficient numerical operations in Python while Pandas is built on top of NumPy and provides high-level data structures and manipulation tools, making it the workhorse for data preparation and Matplotlib is the primary plotting library in Python, used to create static, interactive, and publication-quality visualizations.

These sklearn libraries are essential for data preprocessing and dimensionality reduction in machine learning, ensuring features are scaled properly (0 to 1 or standard deviation 1) and reducing dataset complexity (PCA). They improve model performance, speed up training, and handle different data scales.

2. Import the dataset
The dataset on which you want to work need to be imported , here as i have used cafe-sales-dataset so i will use the cafe-sales-dataset and the command pd.read_csv, here df is the variable in which all the dataset what we perform in commands in stored.

3. Knowing Your Data
When working with real-world data, we rarely get a clean CSV. The process of taking a dataset riddled with missing values, “ERROR” strings, and incorrect data types, and turning it into a reliable source for analysis.

Before fixing anything, you must understand the extent of the “mess.”

Inspecting Structure: Using df.head(), df.tail(), and df.shape to see what the data looks like and how many records exist.

Technical Summary: df.info() reveals a major issue: all columns are detected as object (strings), even the numerical ones like Price and Quantity. This is a red flag that there are non-numeric characters hidden in those columns.
Press enter or click to view image in full size

4. The Big Story Behind Using All These Commands
These command are used to get the overview of our dataset and to check foe flaws and redundancy which need to be corrected first before moving to any further analysis, in our case which have many null values, datatype error, blank cells, typo error s are present.

As we see that price per unit, total spent, quantity colums have missing values we can use simple math to calulate the values that the cell could have and will fill the missing values with those , plus if the redundant rows are less say 50 in a total row of 5000 that we can drop them but if rows are more say 2000 than we need to treat them by proper data substitution using imputation technique.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
To deep dive on how i did all those cleaning of such congested and messy data with 10k plus rows and 9 columns have a look and my blog and do follow me foe further updates :
https://medium.com/@farazmirza57079/data-preprocessing-and-cleaning-on-kaggle-jupiter-notebook-6ffa444c6f53

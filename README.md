# EDA

The plt.rcParams['figure.figsize'] = (10, 6) setting in Matplotlib is used to globally define the default figure size for plots. Here's how it works:

Breakdown:

plt.rcParams['figure.figsize']:--- This modifies the default figure size for all plots.

(10, 6): -----Specifies the width (10 inches) and height (6 inches) of the figure.


To prevent errors, import the warnings module.
The warnings.filterwarnings('ignore') function in Python allows you to suppress all warnings in your code, ensuring a cleaner output.

import warnings
warnings.filterwarnings('ignore')

#for Current directory
import os
os.getcwd()# Get the current Working Directory
#Note 
Note :- To remenber the below Concept
The expression .fillna(np.mean(pd.to_numeric(clean_data['Age']))) is used in pandas to replace missing values (NaN) in the 'Age' column with the mean of the column. Here's how it works:

Breakdown:

pd.to_numeric(clean_data['Age']):--- Converts the 'Age' column to numeric format, ensuring all values are treated as numbers.

#regex
The str.extract('(\d+)') function in pandas is used to extract numeric values from a string column using regular expressions. Here's how it works:

(\d+): This regex pattern captures one or more digits (\d+).

str.extract(): Extracts the first match of the pattern from each row in the column.

Returns a DataFrame with the extracted values.

The expression str.replace(r'\W','',regex=True) is used in pandas to remove all non-word characters from a string column in a DataFrame. Here's how it works:

r'\W': This is a regular expression pattern where:

\W matches any non-word character (anything other than letters, digits, or underscores).

The r'' prefix makes it a raw string, ensuring that backslashes are treated literally.

'': This is the replacement string, meaning all non-word characters will be replaced with an empty string (effectively removed).

regex=True: This tells pandas to interpret the pattern as a regular expression rather than a literal string.

np.mean(...): ---- Computes the mean of the numeric values in the 'Age' column.

.fillna(...):--- Replaces all NaN values with the computed mean.

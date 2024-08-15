### The procedure for loading the Bikeshare data 
# To load the Bikeshare data from the ISLR2 package in R into Python, you can follow this two-step process:
## Step 1: Save the Bikeshare data as a CSV file in R
# Install and load ISLR2 package
install.packages("ISLR2")
library(ISLR2)
# Save Bikeshare data to a CSV file
write.csv(Bikeshare, file = "bike.csv", row.names = FALSE)
# Check the current working directory
getwd()
## Step 2: Load the CSV file into Python
import pandas as pd
# Load the CSV file into a pandas DataFrame
df = pd.read_csv('bike.csv')
# Display the first few rows of the DataFrame
print(df.head())

### We consider the following four models for fitting the Bikeshare data:
M1: LM
M2: Poi-GLM
M3: DNN
M4: Poi-DNN

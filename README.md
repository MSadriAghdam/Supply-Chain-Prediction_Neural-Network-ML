# Supply-Chain-Prediction_Neural-Network-ML
In this dataset, there is some information about the supply chain system of a company and the goal is to predict the best shipment method for new entries.

## Preprocessing:
There are some missing values in this dataset. I replaced the mean(for 'Line Item Insurance (USD)') and mode (for 'Dosage') and removed the rest of the rows for the target column.

### Date columns:
There are 5 date columns in this dataset 'PQ First Sent to Client Date', 'PO Sent to Vendor Date', 'Scheduled Delivery Date', 'Delivered to Client Date', 'Delivery Recorded Date'
2 of them have 23% and 54% missing values while the other 3 do not. I decided to drop those 2 columns and convert those 3 to date-time values using the DateTime function.
Then I extracted the year, month, and day oft of them.

### Numeric features:
About 38% and 96 % of the 'Weight (Kilograms)' and 'Freight Cost (USD)' are not numerical however the rest are numerical. Because of that, I decided to remove these 2 columns.

### High-cardinality columns:
There are some columns in this dataset with a huge number of uncommon and unique values. As getting dummies from these columns can lead the model to misunderstand I decided to remove them. (PQ # ,PO / SO #, ASN/DN # )


### Binary variables:
I replaced binary variables with 0 and 1.

### One hot encoding:
For objects (categorical values) in this dataset, I got dummies and dropped the main columns.

### Split train and test:
Then I split the dataset into train and test and then scaled the training dataset.

### Model:
In this step, I created a Neural Network Model with 2 hidden layers. 771 inputs and 4 outputs (there are 4 different types of shipment methods.)
which the result shows almost 95% of accuracy.
Then I run the model on test data and the result indicates 90.47% accuracy

### confusion matrix:
In the end, I created a confusion matrix to check the result.



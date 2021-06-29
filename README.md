# Supply-Chain-Prediction_Neural-Network-ML
In this dataset there are some information about supply chain system of a company and the goal is to predict the best shipment method for new entries.

## Preprocessing:
There are some missing values in this dataset.I replaced the mean(for 'Line Item Insurance (USD)') and mode (for 'Dosage') and removed the rest of the rows for the target column.

## Date columns:
There are 5 date columns in this dataset 'PQ First Sent to Client Date', 'PO Sent to Vendor Date', 'Scheduled Delivery Date', 'Delivered to Client Date', 'Delivery Recorded Date'
2 of them have 23% and 54% missing values while the other 3 do not. I decided to drop those 2 columns and convert those 3 to date time value using datetime function.
Then I extracted the year, month and day oft of them.

## Numeric features:
About 38% and 96 % of the 'Weight (Kilograms)' and 'Freight Cost (USD)' are not numerical however the rest are numerical. Because of that I decided to remove these 2 columns.

## 


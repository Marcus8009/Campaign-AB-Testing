### Summary of A/B Test Analysis

This notebook performs an A/B test analysis on two groups from a marketing dataset: control and test.

The dataset is from Kaggle: A/B Testing Dataset (https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset).

Here's a summary of the key steps and findings:
#### Steps:

1. **Environment Setup**:
   - Import necessary libraries like `numpy`, `pandas`, and `scipy`.
   - List files in the input directory to ensure data availability.

2. **Data Loading**:
   - Load datasets for control and test groups from CSV files.

3. **Data Merging**:
   - Combine the control and test group data into a single dataframe for analysis.

4. **Data Preparation**:
   - Check for and handle missing values.
   - Convert columns to appropriate data types (e.g., dates, floats, integers).

5. **Data Exploration**:
   - Display the first few rows and summary statistics of the dataframe.

6. **Group Definition**:
   - Separate the combined data into control and test groups based on the campaign name.

7. **A/B Testing**:
   - Perform t-tests on various metrics (e.g., Spend [USD], Impressions, Reach) to compare control and test groups.
   - Calculate t-statistics and p-values to determine if differences are significant.

8. **Results Interpretation**:
   - Print t-statistics, p-values, and conclusions for each metric.

#### Findings:

- **Significant Differences**:
  - **Spending [USD]**: Test group spent less on average.
  - **Number of Impressions**: Test group had more impressions.
  - **Reach**: Test group had higher reach.
  - **Number of Adds to Cart**: Test group had more adds to cart.

- **No Significant Differences**:
  - **Number of Website Clicks**
  - **Number of Searches**
  - **Number of Content Views**
  - **Number of Purchases**

#### Conclusion:

The A/B testing results indicate significant differences between the control and test groups for spending, impressions, reach, and adds to cart. However, there were no significant differences in website clicks, searches, content views, or purchases. The test group did reduce spending, therefore there should be consideration on whether the benefits seen outweigh the costs.

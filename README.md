# IS5126G1

## Data Preprocessing
This dataset contains many columns (362 in total), indicating that it is a fairly complex dataset. Before proceeding with further analysis, we need to identify the preprocessing steps that need to be performed. Common preprocessing steps include:

Handle missing values: Check your data for missing values and decide how to handle them (for example, delete, fill, or impute).
Data type conversion: Ensure that the data type of each column matches its content.
Remove duplicate values: Check and remove duplicate rows if any.
Handle outliers: Check for exceptions or outliers and decide how to handle them.
Feature selection: Consider whether it is necessary to reduce the number of features, especially if there are many features.
Let's start with some basic data checks, including checking for missing values and data types. We can then decide how to proceed further. ​​

There are many columns in this dataset that contain a large number of missing values. For example, some columns have missing values close to or exceeding the total number of rows, which means there is little valid data for these columns. In this case, given the complexity of the dataset and the high degree of missing values, we can consider the following preprocessing steps:

Remove highly missing columns: Remove columns where most of the values are missing.
Handle remaining missing values: For missing values in other columns, consider filling them (for example, using the mean or median) or deleting rows containing missing values.
Check the data type: Make sure the data type of each column is suitable for its content, such as numeric type for numeric data, date type for time data, etc.
Remove duplicate rows: If the exact same row exists in the data set, it should be removed.
First, we can set a threshold, for example, if more than 50% of the data in a column is missing, we will delete this column. Then, further processing is performed on the remaining columns. Let's get started with the steps. ​​

After removing columns with more than 50% missing values, the dataset now contains 242 columns, which is significantly fewer than the original 362 columns. However, there are still some columns that contain a large number of missing values. For these columns, we can decide whether to further delete or fill in missing values based on the specific situation.

Next, we can check the data types to ensure that the type of each column matches its content. We can convert the data type if needed. Additionally, we should also check and remove any duplicate rows.

Since this dataset is financial data, we need to be extra careful with missing values and data types. In some cases, missing values may require special handling, such as using industry-specific filling methods, or remaining as NaN (indicating that the data is not available).

Let's move on to the data type check and see if there are duplicate rows.




Based on common important indicators in finance and economics, I will select 10 representative factors from the dataset provided by you for visualization and descriptive statistical analysis. The basis for selecting these factors is their general importance in financial analysis and their indicative role in a company's financial health. The following are the selected factors and their explanations of importance:

Total fixed assets: Represents the value of a company's long-term investments, important for evaluating a company's capital structure and investment scale.

Interest-free liability: Reflects the level of debt a company does not need to pay interest on, important for evaluating financial pressure.

Interest debt: The total amount of debt a company needs to pay interest on, important for understanding a company's financial costs and debt structure.

Net debt: Total debt minus cash and cash equivalents, a key indicator for measuring a company's financial health.

Operating capital: Current assets minus current liabilities, reflecting a company's short-term financial health.

Operating income: The company's main source of income, an important indicator for evaluating its profitability.

Net profit: Total revenue earned by the company minus total costs, a key indicator for measuring a company's profitability.

Cash flow: Reflects the inflow and outflow of a company's cash, crucial for understanding its operational efficiency.

Return on total assets: Measures a company's asset profitability.

Equity: The residual value of a company's assets minus liabilities, representing the ownership of shareholders in the company.

Next, I will perform visualization and descriptive statistical analysis on these selected factors. Since the column names in the original dataset may not match the above descriptions completely, I will try to match the closest columns. Let's first look at the data for these selected factors.

When attempting to match the selected economic and financial factors, I noticed that the column names in the dataset may not be completely consistent with the provided factor list. I have tried my best to match the closest columns. Since the column names in the dataset may not directly reflect typical financial terms, I have selected some columns that are most relevant to the provided factors.

Since the dataset contains many columns, I have selected several columns that are most relevant to the following factors for analysis:

Total fixed assets
Interest-free liability
Interest debt
Net debt
Equity-related columns


Next, I will perform visualization and descriptive statistical analysis on these selected factors. Since the number of selected columns is relatively large, I will perform visualization in batches to ensure the readability of the charts. First, we will start with visualization.

I have completed visualization and descriptive statistical analysis for the selected five financial factors. The following are the key observations for each factor:

Visualization observations:

Total fixed assets: Most of the data is concentrated in the lower value range, but there are also some extreme cases with higher values.

Interest-free liability: The distribution of this factor is similar to that of total fixed assets, with most values being low, but there are also some high-value cases.

Interest debt: The distribution presents a similar pattern, with most of the data being concentrated in the lower values, but there are extreme high values.

Net debt: The distribution of this factor shows some negative values, which may indicate that some companies hold cash and cash equivalents that exceed their debt.

Equity: Most of the values are low, but there are also some high-value cases. ▌


The image displays a series of histograms and boxplots corresponding to financial data sets: Total fixed assets, Interest debt, Net debt, Operating capital, and Cash and cash equivalent net increase.

**Histograms:**

1. **Total fixed assets:** The histogram is skewed to the right, with most data points concentrated near zero, suggesting most values in the data set are low with a few large outliers.
2. **Interest debt:** This also shows a right-skewed distribution, similar to total fixed assets, indicating that most companies have low interest debt with some exceptions.
3. **Net debt:** The distribution is right-skewed, meaning that most observations are clustered around lower values with few high-value outliers.
4. **Operating capital:** This histogram appears to be more centrally distributed but still shows a slight right-skewness, with most data points close to zero.
5. **Cash and cash equivalent net increase:** The histogram is quite skewed, with a long tail to the right, indicating that while most changes in cash and cash equivalents are small, there are cases with significant increases.

**Boxplots:**

1. **Total fixed assets:** The boxplot indicates a median near zero with a large number of outliers, which are represented by points above the upper whisker.
2. **Interest debt:** Similar to total fixed assets, the median is close to zero with many high-value outliers.
3. **Net debt:** The boxplot shows a median close to zero, with numerous outliers indicating significant variation in net debt among the sampled entities.
4. **Operating capital:** The median operating capital is around zero, with outliers on both sides, suggesting that while many entities have a balance around zero, there are significant deviations in both directions.
5. **Cash and cash equivalent net increase:** The median is slightly above zero, with many outliers above the upper whisker, showing that there are entities with significant increases in cash and cash equivalents.

**Summary and Conclusion:**

The provided financial metrics are highly right-skewed, indicating that a majority of the entities have low values for these financial items, with a small number of entities having very high values. This pattern is commonly seen in financial data where a few entities hold a majority of wealth or debt. The presence of outliers in all the boxplots indicates that there is considerable variability in each financial metric across the entities. The data suggest a financial landscape where most entities maintain conservative levels on these metrics, while a few have much larger scales of operation or debt.
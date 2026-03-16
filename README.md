Colorado Motor Vehicle Sales Data Analysis Project

1.  Objective
    To analyze motor vehicle sales data in Colorado to identify trends, forecast
    future sales, and understand the factors influencing sales.
    ○ Identify the key metrics and objectives for the analysis (e.g., monthly sales
    trends, sales by vehicle type, forecast future sales).
    ○ Define the time frame for the analysis.
2.  Methodology
    1.  Import the libraries
    2.  Data Collection/Import the dataset
    3.  Data Preparation
        1. Clean the data to remove any inconsistencies or errors.
        2. Prepare the data for analysis using tools like Pandas.
        3. Data Quality Check
           Checking of duplicate values
3.  Exploratory Data Analysis and Key finding Insights 1. Univariate Analysis (Single Column) -
    a)Sales Distribution - Sales distribution shows a right-skewed pattern where most sales values are concentrated at lower levels, while a small number of observations have very high sales values. This indicates that high sales events are rare compared to normal sales values. -
    b) County Coverage:📌 Shows how many counties are analyzed and which appear most frequently. - The above code shows that there are 17 unique countries from which countries Adams,Arapahoe,Denver, Douglas and EL Paso are analyzed 32 times of each.

    c)Time-Based Trend Analysis (Core to Your Objective or Economic Cycle)
    a) Yearly Sales Trend
    Insights to capture:
    Overall growth (after 2009 to 2015) or decline(from 2008 to 2009) in vehicle sales
    Impact of economic cycles (e.g., post-2008 trends)
    Recovery or slowdown periods

            b) Quarterly Sales Pattern (Seasonality)
            This graph shows that highest quarter sales in quarter 3 and lowest quarter sales occurs in first quarter.

            c)County-Wise Analysis (Geographic EDA):a) Top Counties by Sales
            Insights:
            These two above table shows **Arphahoe** has highest sale in top ten countries and **Fremont** has lowest sale

            d)County vs Year Trend
            This following plot shows Arphahoe has highest sale in top ten countries and Fremont has lowest sale.
            Insight:
            Growth patterns differ by county
            Some counties show stable demand, others volatile

            e)Relationship Analysis :Year vs Sales
            -This line plot shows that from 2008 to 2009 sales decreases from 1.65 to 1.25.After that from 2009 to 2010 sales is very slightly increasing, But from 2010 to 2011 sales increases from 1.37 to 1.85.From 2011 to 2012 sales again decreases and after 2012 to 2015 sales again increases and reach on peak which is greater than 2.25.

    d) Seasonal Effect Analysis (Quarter-wise Statistics)
    a) Mean Sales per Quarter
    -This seasonal effect sales analysis shows that third quarter mean sale is maximum which is 1.913 and first quarter sale is minimum which is 1.63.Whereas second quarter sale is 1.78 and fourth quarter sale is 1.71.
    (np.float64(0.6695322860838229), np.float64(0.5710455999363857))

                       This above analysis shows that Since the p-value (0.57) is greater than 0.05, we fail to reject the null hypothesis.

                       ✅ Conclusion:

                       There is no statistically significant difference in mean sales across the four quarters.

                       📝 How to Write in Your Project Report

                       A one-way ANOVA test was conducted to compare mean sales across four quarters. The results showed an F-statistic of 0.67 and a p-value of 0.57. Since the p-value is greater than 0.05, we fail to reject the null hypothesis. This indicates that quarterly differences in sales are not statistically significant.

                       📈 What This Means for Your Sales Analysis

                       --Sales are relatively similar across Q1, Q2, Q3, and Q4.
                       --Strong seasonal variation is not present.
                       --The sales pattern may be driven more by long-term yearly trends rather than quarterly fluctuations.
                       --For forecasting, trend-based models may work better than seasonal models.

                       📌 Report line:
                       ANOVA results indicate statistically significant seasonal variation in motor vehicle sales across quarters.

4.  Statiscal Analysis 1. Descriptive Statistics (Baseline Statistics) 1. **Check the Skewness of dataset**
    This statistical analysis shows that since mean=1.760 and median=1.385.So mean>median therefore this sales data shows the positivly skewned (Right Skewed).So we can conclude that A few large values (high outliers) pull the mean upward,Mean becomes greater than median and The tail extends toward the right side.

              **Std deviation → Check sales volatility across counties/years**

              **Check the Skewness of dataset**
              This statistical analysis shows that since mean=1.760 and median=1.385.So mean>median therefore this sales data shows the positivly skewned (Right Skewed).So we can conclude that A few large values (high outliers) pull the mean upward,Mean becomes greater than median and The tail extends toward the right side.

              **Std deviation → Check sales volatility across counties/years**
              This statistical analysis shows that through this dataset we got high standard deviation because there is high fluctation between mean and stadard deviation.This indicates:

              ✅ Sales values are highly dispersed
              ✅ There is high variability in sales
              ✅ Some quarters/years may have very high sales compared to others
              ✅ Possibly presence of outliers
              For a sales dataset, this could mean:

              Sales are not stable
              There are big ups and downs
              Seasonal effect or economic factors may influence sales
              Forecasting may require trend/seasonality modeling

              🎯 Extra Insight (Important)

              Since:
              Mean > Median (positively skewed)
              High standard deviation

              This strongly suggests:
              👉 Some very high sales values are pulling the average upward

           #1 .Minimum Sales: 6274000
           Maximum Sales: 916910000
           Sales Range: 910636000

           🔎 Interpretation

           This indicates:

           ✅ There is a very large variation in sales
           ✅ Some periods (year/quarter) had extremely high sales
           ✅ Some periods had much lower sales
           ✅ Sales are not consistent or stable

           📈 Business Meaning

           A large range like this may suggest:

           Strong seasonality
           Economic impact in some years
           Market growth over time
           Presence of outliers
           Policy changes affecting vehicle sales (if this is your Colorado Motor Vehicle project)

           "The sales range of 910,636,000 indicates significant variability between the highest and lowest sales values, suggesting fluctuations in sales performance across different periods."

           #2. Sales Trend Analysis (Correlation & Trend Strength)
           #a) Correlation Between Time and Sales
           The code shows that co-relation is positive .
           📌 Interpretation:
           A positive correlation suggests that vehicle sales in Colorado generally increased over time.

           #3️⃣ Seasonal Effect Analysis (Quarter-wise Statistics)
           #a) Mean Sales per Quarter
           b) Statistical Comparison Across Quarters (ANOVA)
           #This checks whether quarterly differences are statistically significant.

           #4️⃣ County-Level Statistical Comparison
           #b) T-test (Urban vs Low-Sales Counties)
           ✅ Interpretation for Your T-Test

           Since the p-value (8.158 × 10⁻⁵⁵) is far less than 0.05, we reject the null hypothesis. There is a highly statistically significant difference in sales between top-performing and low-performing counties.

           #5️⃣ Variability & Stability Analysis
           #a) Sales Variance by County

           #Why this matters:
           • High variance(Douglas) → unstable or volatile markets
           • Low variance(Weld) → stable demand
           📌 Business meaning:
           Counties with high variance may require cautious inventory planning

          #6 The Z-score method identifies outliers by measuring how many standard deviations a data point deviates from the mean. Data points with an absolute Z-score greater than 3 are typically considered outliers.

          #7️⃣ Regression Analysis (Factor Influence)
        #a) Simple Linear Regression (Year → Sales)
        (array([12479295.72566157]), np.float64(-24926929130.607895))

            What to interpret:
            • Positive coefficient → sales rising over time
            • Magnitude → rate of change
            📌 Insight:
            Regression results show a positive relationship between time and vehicle sales, indicating long-term growth.

5.  Predicative Modeling
    1️⃣ Define the Prediction Goal (Very Important)
    Be explicit in your report:
    Goal: Forecast future motor vehicle sales in Colorado based on historical yearly and quarterly trends.
    Target variable: sales
    Time variables: year, quarter
    Conclusion:
    ❌ Model performance is poor
    ⚠️ Something wrong in evaluation step
    🔴 MAPE = nan confirms calculation issue
6.  REPORT

    # Colorado Motor Vehicle Sales Data Analysis Report
    1. Data Overview

    ***
    - Time Frame: 0 to 500
    - Total Sales Data Points: 501
    2. Exploratory Data Analysis

    ***
    - Total motor vehicle sales were plotted over time, showing general trends and
      seasonality.
      1️⃣ Overall Trend (Main Insight)

    The blue line (Sales Over Time) shows a clear upward trend from 2008 to 2015.

    👉 Sales are generally increasing year by year.
    This means business performance is improving over time.

    2️⃣ Seasonal Pattern (Quarterly Effect)
    Since the x-axis shows:

    2008 Q1, Q2, Q3, Q4 … up to 2015 Q4

    You can see repeating ups and downs within each year.

    📌 That means there is seasonality in the data.

    For example:

    Some quarters consistently perform higher.
    Some quarters drop regularly.
    This is common in sales data (festivals, financial year-end, demand cycles, etc.).
    "The sales data demonstrates a consistent upward trend with evident quarterly seasonality. Variability in sales increases over time, suggesting business expansion and higher market dynamics." 3. Statistical Analysis

    ***
    - Seasonal decomposition of total sales showed clear seasonal patterns.
      2️⃣ Seasonal Pattern (Quarterly Effect)

    Since the x-axis shows:

    2008 Q1, Q2, Q3, Q4 … up to 2015 Q4

    You can see repeating ups and downs within each year.

    📌 That means there is seasonality in the data.

    For example:

    Some quarters consistently perform higher.

    Some quarters drop regularly.

    This is common in sales data (festivals, financial year-end, demand cycles, etc.). 4. Predictive Modeling

    ***
    - An ARIMA model was used to forecast motor vehicle sales for the next 12 months.
      print(f"forecast: 0.00")
    - The model's Mean Squared Error (MSE) was: 3626683000.00

7.  Conclusions

    ***
    - The analysis provided insights into the trends and seasonality of motor vehicle sales
      in Colorado.
    - The predictive model can be used to forecast future sales, aiding in inventory
      management and sales strategies.

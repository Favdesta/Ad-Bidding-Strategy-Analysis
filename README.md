# Ad Bidding Strategy Analysis: Maximum vs. Average Bidding

## Project Overview
In this project, I conducted a comprehensive data-driven analysis to determine the most effective ad bidding strategy between Maximum Bidding (the traditional approach) and Average Bidding (the new alternative). Working with real advertising performance data over a 40-day period, I leveraged statistical methods and visualization techniques to identify patterns, test hypotheses, and formulate actionable business recommendations.

## Business Context
Digital advertisers constantly seek to optimize their bidding strategies to maximize ROI on ad spend. The Maximum Bidding strategy had been the standard approach, but there was interest in testing whether the Average Bidding strategy could deliver better results in terms of engagement, conversion, and revenue generation. My task was to analyze the A/B test results and provide a data-supported recommendation.

## Data & Methodology

### Dataset
I worked with two datasets tracking 40 days of advertising performance:
- **Control Group**: Maximum Bidding strategy (traditional approach)
- **Test Group**: Average Bidding strategy (new approach)

Each dataset contained key metrics:
- **Impressions**: Number of times ads were displayed
- **Clicks**: Number of user clicks on the ads
- **Purchases**: Number of completed transactions
- **Earnings**: Revenue generated from the ads

### Technical Approach
1. **Data Preparation & Cleaning**:
   - Imported and structured both datasets using pandas
   - Verified data integrity and checked for missing values
   - Combined datasets with appropriate labeling for analysis

2. **Exploratory Data Analysis (EDA)**:
   - Generated comprehensive descriptive statistics for both strategies
   - Created visualizations to identify patterns and differences
   - Calculated derived performance metrics (CTR, CR, CPC, CPP)

3. **Statistical Analysis**:
   - Formulated clear null and alternative hypotheses
   - Performed Shapiro-Wilk tests to verify normality assumptions
   - Conducted independent t-tests to assess statistical significance
   - Calculated Cohen's d to measure effect size and practical significance
   - Determined confidence intervals to estimate true performance differences

4. **Data Visualization**:
   - Created comparative box plots to show metric distributions
   - Developed bar charts with percentage differences for intuitive comparison
   - Built scatter plots to examine relationships between metrics
   - Designed a comprehensive Tableau dashboard featuring:
     - EPC (Earnings Per Click) visualization
     - CTR (Click-Through Rate) trends
     - Conversion Rate (CR) analysis
     - KPI overview panel
     - Click vs. Earnings relationship visualization

## Key Findings

### Performance Metrics Comparison
| Metric | Maximum Bidding | Average Bidding | Difference (%) |
|--------|----------------|-----------------|----------------|
| Impressions | 101,711 | 120,512 | +18.5% |
| Clicks | 5,101 | 3,968 | -22.2% |
| Purchases | 551 | 582 | +5.6% |
| Earnings | $1,909 | $2,515 | +31.8% |

### Efficiency Metrics
| Metric | Maximum Bidding | Average Bidding | Difference (%) |
|--------|----------------|-----------------|----------------|
| Click-Through Rate (CTR) | 5.36% | 3.42% | -36.2% |
| Conversion Rate (CR) | 11.59% | 15.66% | +35.1% |
| Revenue per Click | $0.38 | $0.64 | +68.4% |
| Revenue per Purchase | $3.51 | $4.12 | +17.4% |

### Statistical Significance
- **P-value**: 3.44 × 10^-14 (significantly below the standard 0.05 threshold)
- **Effect Size (Cohen's d)**: 2.07 (considered very large)
- **95% Confidence Interval**: $476 to $737 higher earnings with Average Bidding

## Business Insights

My analysis revealed several critical insights about the two bidding strategies:

1. **Quality vs. Quantity Trade-off**: While Maximum Bidding generated more clicks, Average Bidding produced higher-quality engagement that converted better and generated more revenue.

2. **Conversion Efficiency**: Average Bidding had a 35% higher conversion rate, indicating that it attracted users who were more likely to make purchases.

3. **Revenue Generation**: Average Bidding produced nearly 32% higher earnings despite generating fewer clicks, demonstrating superior revenue efficiency.

4. **Statistical Confidence**: The extremely low p-value (3.44 × 10^-14) and large effect size (Cohen's d = 2.07) provided very strong evidence that the observed differences weren't due to random chance.

5. **ROI Implications**: Average Bidding delivered significantly better return on investment, with each click and impression generating more revenue.

## Recommendations

Based on my comprehensive analysis, I recommended:

1. **Strategy Shift**: Implement the Average Bidding strategy as the primary approach for ad campaigns, given its superior performance in generating revenue and conversions.

2. **Phased Implementation**: Roll out the new strategy gradually across campaigns, allowing for continuous monitoring and verification of performance in different market segments.

3. **Metric Prioritization**: Focus on conversion rates and earnings rather than raw click volumes when evaluating campaign success.

4. **Further Testing**: Consider additional A/B tests with larger sample sizes and across different product categories to validate findings and optimize implementation.

## Business Impact

The implementation of my recommendations was projected to deliver:
- Approximately 30% increase in ad-generated revenue
- Improved marketing efficiency with better conversion rates
- More cost-effective customer acquisition
- Enhanced overall ROI on advertising spend

## Technical Skills Demonstrated

- **Python Data Analysis**: Utilized pandas, NumPy, SciPy for data manipulation and statistical analysis
- **Data Visualization**: Created insightful visualizations using Matplotlib, Seaborn, and Tableau
- **Statistical Methods**: Applied hypothesis testing, significance testing, and effect size calculation
- **A/B Testing**: Designed and analyzed experiments to compare strategy performance
- **Business Analytics**: Translated technical findings into actionable business recommendations

## Tableau Dashboard

My interactive Tableau dashboard featured five key components:

https://public.tableau.com/shared/DDTWBRXTD?:display_count=n&:origin=viz_share_link 

1. **EPC (Earnings Per Click) Visualization**: Compared the revenue efficiency of each click between strategies
2. **CTR (Click-Through Rate) Analysis**: Visualized impression-to-click conversion differences
3. **CR (Conversion Rate) Comparison**: Highlighted the superior purchase conversion of Average Bidding
4. **KPI Overview Panel**: Provided at-a-glance performance metrics for both strategies
5. **Click vs. Earnings Scatter Plot**: Demonstrated the relationship between engagement and revenue

The dashboard enabled stakeholders to interact with the data, filter by date ranges, and explore the performance metrics in depth, facilitating informed decision-making based on data-driven insights.

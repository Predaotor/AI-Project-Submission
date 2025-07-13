# Employee Sentiment Analysis and Flight Risk Prediction

## Overview

This project analyzes employee email data to extract sentiment, rank employees, identify potential flight risks, and predict future sentiment trends using machine learning models. The analysis provides insights into employee engagement and helps organizations proactively address retention issues.

## Project Structure

```
AI-project-submission/
├── data/
│   ├── test(in).csv                 # Input dataset
│   └── processed_data_with_sentiment.csv  # Processed data with sentiment labels
├── notebooks/
│   └── employee_sentiment.ipynb     # Main analysis notebook
├── visualizations/
│   └── charts/                      # All generated plots and charts
├── reports/
│   └── final_report.docx            # Detailed project report
├── PROJECT_INSTRUCTIONS.md          # Project requirements
├── README.md                        # This file
└── requirements.txt                 # Python dependencies
```

## Tasks Completed

### ✅ Task 1: Sentiment Labeling
- **Approach**: Used VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analyzer
- **Output**: Assigned positive, neutral, and negative labels to all employee messages
- **Method**: Compound score thresholds (Positive: ≥0.05, Negative: ≤-0.05, Neutral: -0.05 to 0.05)

### ✅ Task 2: Exploratory Data Analysis (EDA)
- **Data Structure Analysis**: Comprehensive dataset overview and quality assessment
- **Sentiment Distribution**: Analyzed sentiment patterns across the organization
- **Time Series Analysis**: Monthly sentiment trends and seasonal patterns
- **Employee-Level Analysis**: Individual employee engagement patterns
- **Message Content Analysis**: Correlation between message characteristics and sentiment
- **Visualizations**: Generated 7+ charts for comprehensive insights

### 🔄 Task 3: Employee Score Calculation (In Progress)
- **Monthly Aggregation**: Calculate sentiment scores per employee per month
- **Scoring System**: Positive (+1), Negative (-1), Neutral (0)
- **Reset Logic**: Scores reset at the beginning of each month

### 🔄 Task 4: Employee Ranking (In Progress)
- **Top Positive Employees**: Identify employees with highest sentiment scores
- **Top Negative Employees**: Identify employees with lowest sentiment scores
- **Monthly Rankings**: Generate monthly employee rankings

### 🔄 Task 5: Flight Risk Identification (In Progress)
- **Risk Criteria**: Employees with 4+ negative messages in 30-day rolling window
- **Early Warning System**: Identify potential retention issues
- **Risk Visualization**: Generate flight risk indicators

### 🔄 Task 6: Predictive Modeling (In Progress)
- **Feature Engineering**: Message frequency, length, word count, sentiment patterns
- **Model Development**: Linear regression and advanced ML models
- **Performance Evaluation**: RMSE, MAE, R² metrics
- **Predictive Insights**: Forecast employee sentiment trends

## Key Findings

### Sentiment Distribution
- **Overall Sentiment**: [To be populated from analysis results]
- **Positive Messages**: [X%] - Indicates [good/poor] employee morale
- **Negative Messages**: [Y%] - Highlights areas of concern
- **Neutral Messages**: [Z%] - Standard communication patterns

### Employee Engagement Patterns
- **Most Active Employees**: [To be populated from analysis]
- **Sentiment Leaders**: [To be populated from analysis]
- **Engagement Trends**: [To be populated from time series analysis]

### Message Characteristics
- **Average Message Length**: [X] characters
- **Word Count Patterns**: [Y] words per message
- **Sentiment-Length Correlation**: [Positive/Negative/No correlation]

## Visualizations Generated

All visualizations are automatically saved to `visualizations/charts/`:

### Sentiment Analysis
- `sentiment_distribution.png` - Pie and bar charts of sentiment distribution
- `monthly_sentiment_trends.png` - Time series of sentiment over months
- `monthly_sentiment_percentages.png` - Sentiment percentage trends

### Employee Analysis
- `employee_message_distribution.png` - Distribution of messages per employee
- `message_length_analysis.png` - Message length by sentiment category

### Statistical Analysis
- `correlation_matrix.png` - Variable correlation heatmap
- `sentiment_length_boxplot.png` - Message length distribution by sentiment

## Technical Implementation

### Technologies Used
- **Python 3.8+**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NLTK**: Natural language processing and VADER sentiment analysis
- **Matplotlib/Seaborn**: Data visualization
- **NumPy**: Numerical computations
- **Scikit-learn**: Machine learning models (for upcoming tasks)

### Key Functions
- **Sentiment Analysis**: VADER-based labeling with custom thresholds
- **Data Processing**: Automated column detection and error handling
- **Visualization Pipeline**: Automated chart generation and saving
- **Statistical Analysis**: Comprehensive EDA with insights generation

## Recommendations

### For HR Teams
- **Real-time Monitoring**: Implement sentiment analysis dashboards
- **Proactive Intervention**: Use flight risk indicators for early intervention
- **Engagement Programs**: Focus on employees showing declining sentiment

### For Management
- **Monthly Reviews**: Regular sentiment trend analysis
- **Resource Allocation**: Direct retention efforts based on risk indicators
- **Communication Strategy**: Adapt messaging based on sentiment patterns

### For Data Teams
- **Model Integration**: Deploy predictive models in production
- **Continuous Learning**: Update models with new data
- **Feature Enhancement**: Incorporate additional data sources

## Reproducibility

### Quick Start
1. **Clone the repository**:
   ```bash
   git clone [repository-url]
   cd AI-project-submission
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis**:
   ```bash
   cd notebooks
   python employee_sentiment.py
   ```

### Data Requirements
- Input file: `data/test(in).csv`
- Expected columns: employee_id, date, message (or similar text column)
- Format: CSV with UTF-8 encoding

### Output Files
- **Processed Data**: `data/processed_data_with_sentiment.csv`
- **Visualizations**: `visualizations/charts/*.png`
- **Analysis Results**: Console output with detailed insights

## Limitations & Future Work

### Current Limitations
- **Sentiment Model**: VADER may not capture domain-specific nuances
- **Feature Scope**: Limited to message metadata (future: content analysis)
- **Temporal Analysis**: Monthly aggregation (future: daily/weekly trends)

### Future Enhancements
- **Advanced NLP**: Domain-specific sentiment model training
- **Social Network Analysis**: Email communication patterns
- **Topic Modeling**: Content-based sentiment insights
- **Real-time Processing**: Streaming sentiment analysis
- **Multi-modal Analysis**: Combine email with other communication channels

## Contributing

This project follows standard data science workflows:
1. **Data Exploration**: Understand the dataset structure
2. **Feature Engineering**: Create relevant features
3. **Model Development**: Build and validate models
4. **Insight Generation**: Extract actionable insights
5. **Documentation**: Maintain clear documentation

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For questions or contributions, please refer to the project documentation or create an issue in the repository.

---

**Note**: This README will be updated with specific findings and results as the analysis progresses through all six tasks. Current focus is on completing Tasks 3-6 and populating the key findings with actual data insights.



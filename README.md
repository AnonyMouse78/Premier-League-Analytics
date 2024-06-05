# Premier-League-Analytics

## Overview

This project focuses on predicting the outcomes of football matches in the English Premier League (EPL). By leveraging data scraping techniques and machine learning algorithms, we aim to accurately forecast match winners based on historical match data.

## Project Structure

### Data Scraping: Utilize requests, BeautifulSoup, and pandas to collect match data from FBref.
- Fetch the HTML content of EPL match pages using the requests library.
- Parse the HTML to extract relevant match data using BeautifulSoup.
- Store the extracted data in a pandas DataFrame for further processing.

### Data Cleaning: Process and clean the scraped data to prepare it for machine learning models using pandas
- Load the scraped match data.
- Perform data cleaning operations, such as handling missing values and converting data types.
- Engineer features that are relevant for predicting match outcomes.

### Prediction Modeling: Apply machine learning techniques using scikit-learn to predict match outcomes
- Define the target variable and features for the machine learning model.
- Train a Random Forest Classifier to predict match winners.
- Evaluate the model's performance using accuracy and precision metrics.

### Model Evaluation: Measure the accuracy of predictions and implement improvements to enhance model performance
- Analyze the model's predictions to identify areas for improvement.
- Implement advanced techniques, such as rolling averages, to enhance prediction accuracy.
- Re-train and re-evaluate the model to measure performance gains.

## Local Setup

### Dependencies
To set up this project locally, ensure you have the following installed:
- JupyterLab
- Python 3.8+
- Python Packages:
  - pandas
  - requests
  - beautifulsoup4
  - scikit-learn
 
### Data
In the first part of this project (scraping.ipynb), we gather match data from FBref using web scraping techniques. The data is saved into a file named matches.csv, which is then used for building and evaluating prediction models in the second part (predictions.ipynb).

## Key Insights

- Home Field Advantage: Matches played at home significantly increase the chances of winning, highlighting the importance of venue in match outcomes.
- Recent Performance: Rolling averages of recent matches are strong indicators of future performance, with teams performing well in recent games more likely to continue winning.
- Opponent Strength: The strength and form of the opponent play a crucial role in predicting match outcomes, with certain teams consistently performing better or worse against specific opponents.
- Prediction Accuracy: The Random Forest model achieved a precision score of 62% in predicting match winners, indicating a reasonable level of accuracy that can be further improved.
- Seasonal Variations: There are notable differences in team performance and match outcomes across different seasons, emphasizing the need to include data from multiple seasons for better predictions.

## Conclusion

This project effectively demonstrates the prediction of English Premier League match outcomes using data scraping and machine learning techniques. By leveraging Python and various data analysis libraries, we collected, cleaned, and processed match data from FBref, resulting in a comprehensive dataset for analysis.

Key insights from our analysis reveal significant factors influencing match outcomes, such as home field advantage, recent team performance, opponent strength, and match timing. Our Random Forest model achieved a precision score of 62%, highlighting the model's capability to make reasonably accurate predictions. Through the implementation of rolling averages and feature engineering, we identified patterns in team performance that contribute to better predictive accuracy. The analysis also underscores the importance of incorporating data from multiple seasons to account for seasonal variations in team performance.

Ultimately, this project provides valuable insights into the factors that determine match outcomes in the English Premier League, equipping stakeholders with the tools to make data-driven decisions. There are ample opportunities for further enhancement, including expanding the dataset, experimenting with additional features, and exploring different machine learning algorithms to improve prediction accuracy.

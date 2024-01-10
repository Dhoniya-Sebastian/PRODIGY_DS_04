# PRODIGY_DS_04

**Problem statement:** Analyse and visualize sentiment patterns in social media data to understand public opinions and attitude towards specific topic or brands.

***1. Data Loading and Inspection:***

It starts by importing necessary libraries: pandas, numpy, matplotlib.pyplot, seaborn, and plotly.express.
The dataset is loaded from a CSV file named 'threads_reviews.csv' using Pandas, and the first few rows, shape, and information about the dataset are displayed.

***2. Data Cleaning:***

The script checks for and removes duplicate rows in the dataset.
The distribution of ratings and sources is visualized using Seaborn.

***3. Data Visualization:***

Various visualizations are created using Matplotlib and Seaborn to understand the distribution of ratings and sources, as well as the distribution of review dates.
Word clouds are generated for each rating category using the WordCloud library, providing a visual representation of frequently occurring words in reviews with different ratings.

***4. Text Cleaning:***

The script installs the emoji library and defines a function (cleaning_text) to clean the text data in the 'review_description' column. This function converts text to lowercase, removes numbers, and converts emojis to text.

***5. Text Preprocessing:***

The script installs the nltk library and performs tokenization and stemming on the cleaned text data. It uses the Porter Stemmer from NLTK to find word roots.

***6. Sentiment Analysis:***

The script installs the textblob library, and sentiment analysis is performed on the stemmed text using the TextBlob library. Two new columns, 'subjectivity' and 'polarity', are added to the dataset.
Sentiment classes (positive, negative, neutral) are assigned based on the polarity scores.

***7. Visualization of Sentiment Analysis:***

Bar plot visualizes the distribution of sentiment classes.
Scatter plot shows the relationship between polarity and subjectivity in the reviews.

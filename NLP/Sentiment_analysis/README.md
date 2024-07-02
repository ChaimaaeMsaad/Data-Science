# Sentiment Analysis Streamlit App

This Streamlit application performs sentiment analysis on text input using various natural language processing techniques and visualizes the results. It utilizes TextBlob for sentiment analysis, VaderSentiment for token-level sentiment analysis, and Altair for data visualization.

## Features 
* Sentiment Analysis: Analyzes the sentiment (polarity and subjectivity) of the entered text using TextBlob.
* Token-level Sentiment: Provides a breakdown of sentiment for individual tokens using VaderSentiment.
* Visualization: Visualizes sentiment metrics using interactive charts created with Altair.

## How to Run
### Install Dependencies:
Ensure you have installed the necessary libraries:

```bash
pip install streamlit textblob pandas altair vaderSentiment
```

### Run the Application:

  * Open your terminal or command prompt.
  *  Navigate to the directory containing sentimentanalysis.py.
  * Execute the following command:

```bash
streamlit run sentimentanalysis.py
```

### Interact with the App:

  * Once the app is running locally, a browser window will open automatically, or you can access it at ``` http://localhost:8501```
  * Enter text into the provided text area and click Analyze to see sentiment analysis results and visualizations.





    


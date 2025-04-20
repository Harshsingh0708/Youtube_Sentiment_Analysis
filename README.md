# Youtube_Sentiment_Analysis
🧠 Project Overview: YouTube Sentiment Analysis Related to AI & Data Science
This project focuses on performing sentiment analysis on YouTube comments related to Artificial Intelligence (AI) and Data Science. The primary goals include:

Extracting user comments from YouTube videos using the YouTube Data API.

Preprocessing and cleaning the collected text data.

Performing sentiment analysis using the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool.

Visualizing sentiment distributions and drawing conclusions about public perception towards AI and Data Science.

Key Objectives:

Understand public sentiment toward trending AI and Data Science topics.

Gain hands-on experience working with APIs, text data, NLP tools, and visualization techniques.

Develop a reusable pipeline for YouTube sentiment analysis.

🛠️ Setup Instructions
To run this project successfully on your local machine, follow these steps:

1. Clone or Download the Repository
bash
Copy
Edit
git clone <repository-link>
cd youtube-sentiment-analysis
Replace <repository-link> with your actual repository URL if hosted on GitHub or any version control system.

2. Install Required Libraries
Make sure Python 3.7+ is installed. Then install dependencies:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn nltk google-api-python-client vaderSentiment wordcloud
For Jupyter Notebook users:

bash
Copy
Edit
pip install notebook
3. NLTK Resource Downloads
The project uses VADER from the nltk library, so you’ll need to download it:

python
Copy
Edit
import nltk
nltk.download('vader_lexicon')
4. API Key Configuration
To use the YouTube Data API, you'll need a valid API key from Google Developers Console:

Create a project and enable the YouTube Data API v3.

Generate an API key.

Add your key in the notebook where specified:

python
Copy
Edit
api_key = 'YOUR_YOUTUBE_API_KEY'
▶️ Usage Guidelines
Step-by-Step Execution:
YouTube Comment Extraction

The script fetches comments from a specified video URL using googleapiclient.discovery.

Modify the video ID list to analyze different videos related to AI and Data Science.

Data Cleaning and Preprocessing

Converts text to lowercase.

Removes punctuation, numbers, and stopwords.

Applies basic tokenization.

Sentiment Analysis

Uses the VADER SentimentIntensityAnalyzer to classify text as Positive, Neutral, or Negative.

Scores are visualized using bar charts and pie charts.

WordCloud Generation

Generates word clouds to visualize the most common terms in positive, neutral, and negative comments.

Insights & Interpretation

The notebook concludes with a summary of the sentiment analysis findings and potential implications regarding public perception of AI and Data Science topics.

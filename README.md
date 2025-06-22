# Canada-USA Tariff Sentiment Analysis

This project performs sentiment analysis on media articles related to Canada-USA trade and tariff issues using RoBERTa from Hugging Face's `transformers`. The workflow includes web scraping, sentiment classification, Google Drive storage, and Power BI dashboard visualization.

## Model Used

- Model: cardiffnlp/twitter-roberta-base-sentiment
- Library: Hugging Face `transformers` (pipeline-based)

## Features

- Scrape articles using:
  - newspaper3k (preferred)
  - BeautifulSoup + requests (fallback)
- Sentiment classification (Positive, Neutral, Negative)
- CSV storage on Google Drive
- Word clouds and sentiment distribution visualizations using:
  - matplotlib, seaborn, wordcloud
- Power BI dashboard for reporting insights

## Project Structure

.
├── sentiment_analysis.py
├── requirements.txt
├── README.md
├── .gitignore
├── article_links.csv
├── SentimentResults.csv
└── visualizations/
    ├── sentiment_distribution.png
    └── wordcloud.png

## Setup

1. Clone the repo:
   git clone https://github.com/ronaldkalani/TariffSentimentAnalysis.git
   cd canada-usa-tariff-sentiment

2. Install dependencies:
   pip install -r requirements.txt

3. (Optional - Google Colab)
   Mount Google Drive:
   from google.colab import drive
   drive.mount('/content/drive')

4. Run the sentiment pipeline:
   python sentiment_analysis.py

## Visualizations

Exported images and .csv are ready for Power BI import. Dashboard includes:

- Sentiment KPI cards  
- Word clouds  
- Source-based sentiment charts  
- Article table with filters

## References

- Hugging Face RoBERTa Model: https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment
- Newspaper3k Documentation: https://newspaper.readthedocs.io/
- Power BI Docs: https://learn.microsoft.com/en-us/power-bi/



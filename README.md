# SocioSentiment
🧠 SocioSentiment – Social Issue Sentiment & Emotion Analyzer

SocioSentiment is a Streamlit-powered web application designed to examine text related to social topics and determine both sentiment (Positive, Neutral, or Negative) and emotional tone (such as joy, anger, fear, sadness, or surprise). The system uses pre-trained Transformer models from Hugging Face that have been fine-tuned for sentiment and emotion classification tasks.

🤖 Models Used

cardiffnlp/twitter-roberta-base-sentiment → Detects overall sentiment

j-hartmann/emotion-english-distilroberta-base → Identifies the emotional category expressed in the text

⚙ How the System Operates

The user submits a sentence through the web interface.

The application preprocesses the text by removing noise such as URLs, mentions, and unnecessary characters.

The cleaned text is tokenized into numerical representations suitable for machine learning models.

Transformer models perform inference on the input (the models are not retrained during runtime).

A Softmax layer converts the model outputs into probability values.

The application then displays:

Predicted sentiment and emotion labels

Confidence scores for each prediction

Probability distribution visualizations

Important keywords extracted using TF-IDF

🚀 Main Features

Utilizes transfer learning through Hugging Face transformer models

Real-time text analysis directly in the web interface

Visualization of prediction confidence for better interpretability

Keyword extraction to highlight influential terms in the input text

Faster performance using Streamlit’s st.cache_resource

🔮 Planned Enhancements

Statistics Dashboard – Summarize trends and insights from multiple analyzed texts

Live Issue Monitoring – Connect with NewsAPI to automatically analyze current social topics

CSV Export – Allow users to download analysis results for offline use

Emoji Sentiment Detection – Interpret emojis as part of emotional context

Multilingual Capability – Detect languages such as German, Portuguese, French, and Hinglish

Automatic Translation – Convert detected non-English text to English before analysis

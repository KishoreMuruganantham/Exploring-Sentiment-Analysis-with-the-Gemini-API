# Sentiment Analysis with Gemini API 🎯✨🌟

Welcome to the **Sentiment Analysis** project! This repository leverages the power of the **Gemini API** to analyze text sentiment and classify it into positive, negative, or neutral categories. The goal is to demonstrate how advanced AI models can be used to extract meaningful insights from textual data, such as customer reviews, product feedback, or social media posts. 🌍🔍💡

---

## Features 🚀📊🔧

- 🌟 Sentiment analysis of reviews with detailed score probabilities.
- 📦 JSON response schema for easy integration into applications.
- 🛠️ Simple, reusable, and adaptable code structure.

---

## Setup Instructions 🛠️📋💾

### Prerequisites 🐍🔑📥

- 🐍 Python 3.7+
- 🔑 An active Google Gemini API key.
- 📥 Required Python libraries (installed via pip):
  ```bash
  pip install google-generativeai
  ```

### Setting Up the API Key 🔐💾📝

For best practices in API key security, consider using environment variables or a secrets manager to store your API key securely. Avoid hardcoding the key directly into your scripts to minimize the risk of accidental exposure.

1. 🔐 Obtain your API key from the Google Developer Console.
2. 💾 Store the API key securely in your environment and access it in the notebook:
   ```python
   from google.colab import userdata
   GOOGLE_API_KEY = userdata.get('GOOGLE_API_KEY')
   genai.configure(api_key=GOOGLE_API_KEY)
   ```

---

## Usage 🖥️📂⚙️

### Steps to Run 📋🚀🖱️

1. 📂 Clone this repository and install dependencies:
   ```bash
   git clone https://github.com/KishoreMuruganantham/Exploring-Sentiment-Analysis-with-the-Gemini-API.git
   cd <repository-folder>
   pip install -r requirements.txt
   ```
3. 📝 Open the notebook `Sentiment_Analysis.ipynb` in Jupyter Notebook or Google Colab.
4. 🚀 Follow the cell-by-cell instructions to analyze the sentiment of predefined or custom text inputs.

---

## How It Works 🧠📨📊

1. 🧠 The model processes a given review (e.g., "This was one of the worst experiences...").
2. 📨 A prompt is sent to the Gemini API to generate sentiment scores.
3. 📊 The API returns a structured JSON response with probabilities for each sentiment:
   ```json
   {
       "positive_sentiment_score": 0.2,
       "negative_sentiment_score": 0.1,
       "neutral_sentiment_score": 0.7
   }
   ```

---

## Example Output 🌟📊📝

### Input Review:
> "I can’t recommend this enough! A perfect blend of value and quality that left me completely satisfied."

### JSON Output:
```json
{
    "positive_sentiment_score": 0.95,
    "negative_sentiment_score": 0.05,
    "neutral_sentiment_score": 0.0
}
```

---

## Applications 📝📈💬

- 📝 Analyze customer feedback (e.g., restaurant reviews, product comments).
- 💬 Evaluate sentiment in social media posts or emails.
- 📈 Generate insights for market research.

---

## Contributing 🌟📥🔧

Contributions are welcome! If you have suggestions or improvements, feel free to submit a pull request. 🎉🤝📂

---

## License 📝🔓📜

This project is licensed under the GNU Affero General Public License Version 3. See the `LICENSE` file for details. 📄✨🔑

---

### Explore More 📚🔎✨

Check out additional notebooks in this repository for more advanced use cases and customizations of the Gemini API! 🌌🖥️💡

